# Shorter

_You can always be shorter._

Shorter is a simple URL shortener written in Rust. It stores the urls in-memory or in a file.

I am using bpaf to parse the command line arguments and some essential features to deliever the good cli experience.

## How it works?

Shorter uses a simple algorithm to generate the shortened version of the URL. It uses the first 6 characters of the SHA256 hash of the URL. It is not a secure way to generate the shortened version of the URL, but it is simple and easy to implement. It is also easy to remember the shortened version of the URL.

It will save the shortened version of the URL and original URL in a file or in-memory.

## Usage

```
Usage: -s UID -g UID -d UID [-l] [-f FILE]

Available options:
    -s, --save <UID>    Save a url
    -g, --get <UID>     Get a url
    -d, --delete <UID>  Delete a url
    -l, --list          List all urls
    -f, --file <FILE>   File to save to
    -h, --help          Prints help information
```

## Build

```
cargo build --release
```

## Test

```
cargo test
```

### To myself

- pathbuf: todo!
- closure: todo!
- serde: todo!
- construct! todo!

## License

This project is licensed under the terms of the MIT license.
