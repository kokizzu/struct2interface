# struct2interface

struct2interface is a CLI utility to extract an interface from a Golang struct

## Installation

```bash
go get github.com/reflog/struct2interface
```

## Usage

```bash
struct2interface --help

Usage:
  struct2interface [flags]

Flags:
  -f, --folder string      Path to the package in which the struct resides
  -h, --help               help for struct2interface
  -i, --interface string   Name of the output interface
  -o, --output string      Path to output file (will be overwritten)
  -p, --package string     Name of the package in which the struct resides
  -s, --struct string      Name of the input struct
  -t, --template string    Path to a Go template file to use for writing the resulting interface

struct2interface -f "/home/reflog/go/src/github.com/mattermost/mattermost-server/app" -o "/home/reflog/go/src/github.com/mattermost/mattermost-server/
app/app_iface.go" -p "app" -s "App" -i "AppIface"
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)