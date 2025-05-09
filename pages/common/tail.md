# tail

> Display the last part of a file.
> See also: `head`.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/tail-invocation.html>.

- Show last 'count' lines in file:

`tail {{[-n|--lines]}} {{count}} {{path/to/file}}`

- Print a file from a specific line number:

`tail {{[-n|--lines]}} +{{count}} {{path/to/file}}`

- Print a specific count of bytes from the end of a given file:

`tail {{[-c|--bytes]}} {{count}} {{path/to/file}}`

- Print the last lines of a given file and keep reading it until `<Ctrl c>`:

`tail {{[-f|--follow]}} {{path/to/file}}`

- Keep reading file until `<Ctrl c>`, even if the file is inaccessible:

`tail {{[-F|--retry --follow]}} {{path/to/file}}`

- Show last 'num' lines in 'file' and refresh every 'n' seconds:

`tail {{[-n|--lines]}} {{count}} {{[-s|--sleep-interval]}} {{seconds}} {{[-f|--follow]}} {{path/to/file}}`
