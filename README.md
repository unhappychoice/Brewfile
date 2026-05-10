# Brewfile

My personal [Homebrew](https://brew.sh/) package list, managed with
[homebrew-file](https://github.com/rcmdnk/homebrew-file).

## Structure

The `Brewfile` is split into three sections:

- **common** — cross-platform formulae installed on every machine
  (modern CLI tools, git tooling, runtime managers, etc.)
- **macOS** (`if OS.mac?`) — formulae, casks, and Mac App Store apps
- **Linux** (`if OS.linux?`) — Linux-only formulae

## Usage

Install [brew-file](https://github.com/rcmdnk/homebrew-file) first, then point
it at this repository:

```sh
brew install rcmdnk/file/brew-file
brew file set_repo unhappychoice/Brewfile
brew file install
```

Sync changes:

```sh
brew file update   # apply Brewfile to the system
brew file pull     # pull latest from the repo
brew file push     # push local changes
```

## License

[MIT](./LICENSE)
