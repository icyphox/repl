# repl
> an instant REPL for any command

## Features
- Command history (cycle with arrow keys)
- It's epic

## Installation

Assuming `$HOME/bin` is in your `$PATH`,
```console
curl -s https://raw.githubusercontent.com/icyphox/repl/master/repl -o bin/repl
```

## Usage

It's simple, just `repl <command>`.

```console
$ repl git
git% branch
* master
git% remote -v
origin  git@github.com:icyphox/asdf (fetch)
origin  gitgit@github.com:icyphox/asdf (push)
git% 
```

Or, pipe it to STDIN — `repl --stdin <command>`.

```console
$ repl --stdin cat
cat% 
yeet
cat% fortnite bad, mc good
fornite bad, mc good
```
And here's `repl` being used with `ed(1)` :)

```console
$ repl --stdin ed
ed% what
?

ed% am
?

ed% i

ed% doing
?

ed% 
```

## License
MIT © [Anirudh Oppiliappan](https://icyphox.sh)
