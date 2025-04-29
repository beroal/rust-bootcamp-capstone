Ideas for my capstone project for the Rust Bootcamp — Winter 2025.

# Dense passphrase

A program for generating dense passphrases.
A passphrase is an access key in the form of a list of words that humans are supposed to remember and type into a computer.
While passphrases are easier to remember than passwords, they are also longer (entropy values being equal).
Dense passphrases are expected to be approximately two times shorter than usual passphrases with the same entropy.
This is useful if the password length is limited or you want to type passwords faster.
Length shortening is achieved by filtering out frequent letters and taking a fixed-length prefix of each word.
The Rust program will consist of the dictionary builder and the passphrase generator.
The dictionary builder helps users prepare a dictionary and find optimal dictionary parameters.
The passphrase generator randomly and securely generates passphrases for requested entropy using a dictionary.

# BitTorrent media streaming

A plugin for a BitTorrent client that streams media to a local media player.
The plugin sends media fragments as soon as they are downloaded via BitTorrent
so a user can start watching a movie immediately after starting downloading it.
The plugin will be embedded into a client written in Rust.
The plugin will support jumping to any point in media.
Media will be streamed via HTTP.
Actually, one of BitTorrent clients (rqbit) already [does this](https://github.com/ikatson/rqbit#streaming-support),
but others
([synapse](https://github.com/Luminarys/synapse),
[Vincenzo](https://github.com/gabrieldemian/vincenzo),
[naryand/bittorrent](https://github.com/naryand/bittorrent),
[RustyBit](https://github.com/h33333333/rustybit),
[Rubit](https://github.com/spectre-xenon/rubit),
[Rusty Torrenter](https://github.com/ArloFilley/rusty_torrent#rusty-torrenter),
[xerus](https://gitlab.com/zenoxygen/xerus))
don't.

# Indented bracketed expressions

A text format based on Lisp S-expressions.
S-expressions are infamous for their large number of parentheses.
Indented bracketed expressions allow to replace parentheses with indentations.
Indented bracketed expressions are suitable for rapidly designing syntax for programming languages, configuration files, rich text, small databases, and network messages.
Other features of the format are:

- **Code in text.** Useful for string interpolation in programming languages and rich text.
- **Minimal.** Syntax constructs that may be parsed further is not included.
- **Defined with formal languages.**

The Rust program will consist of the parser and the pretty printer.

delme

