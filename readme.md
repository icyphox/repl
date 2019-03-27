# repl
> an instant REPL for any command

## Features
- Command history (cycle with arrow keys)
- Reverse-search using `Ctrl+R`
- It's epic

## Requirements
- `bash`
- `rlwrap` (optional, needed for history)

## Installation

Assuming `$HOME/bin` is in your `$PATH`,
```console
curl -s https://raw.githubusercontent.com/icyphox/repl/master/repl -o $HOME/bin/repl
chmod +x $HOME/bin/repl
```

## Usage

It's simple, just `repl <command>`:

```console
$ repl git
git% branch
* master
git% remote -v
origin  git@github.com:icyphox/asdf (fetch)
origin  gitgit@github.com:icyphox/asdf (push)
```

Or, pipe it to STDIN — `repl --stdin <command>`:

```console
$ repl --stdin cat
cat% 
yeet
cat% fortnite bad, mc good
fornite bad, mc good
```

Reverse-search by hitting `Ctrl+R`:

```console
$ repl pip3
(reverse-i-search)`li': list
```

And here's `repl` for `ed(1)` :)

```console
$ repl --stdin ed
ed% what
?

ed% am
?

ed% i

ed% doing
?
```

## Prior art

[`repl(1)`](https://github.com/defunkt/repl) by [Chris Wanstrath](https://github.com/defunkt)

## License
MIT © [Anirudh Oppiliappan](https://icyphox.sh)
