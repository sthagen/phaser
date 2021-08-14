<p align="center">
  <img alt="Phaser logo" src="https://kerkour.com/imgs/phaser.svg" height="200" />
  <h1 align="center">Phaser</h1>
  <h3 align="center">Automated attack surface mapper and vulnerability scanner</h3>
</p>



## What is this?

Phaser is a high-performance and automated attack surface mapper and vulnerability scanner. Just point it to a target, and it will autimagically generate a report with everything it can finds, saving you hours of manual audit and pipping between different tools.


![Architecture](https://raw.githubusercontent.com/skerkour/phaser/main/docs/phaser_architecture.svg)


Want to learn how to use Rust to hack the planet? Phaser was extracted and improved from the chapters 2, 3, and 4 of my book [Black Hat Rust](https://academy.kerkour.com/black-hat-rust?coupon=PHASER), where, among other things, we learn how to build a fast async scanner.

<div align="center">
  <a href="https://academy.kerkour.com/black-hat-rust?coupon=GITHUB" target="_blank" rel="noopener">
    <img alt="Black Hat Rust logo" src="https://kerkour.com/imgs/black_hat_rust_cover.svg" height="300" />
  </a>

  <h3>
    <a href="https://academy.kerkour.com/black-hat-rust?coupon=PHASER">Buy the book now!</a>
  </h3>
</div>

One of the goals of phaser is to get you started once you finish the book. Either by helping you make your first Rust contribution, or by using it in your first bug hunting session.


## Installation

### Using cargo

```shell
$ cargo install -f phaser
```


### Using Docker

```shel
$ docker pull ghcr.io/skerkour/phaser
```


## Usage

```shell
# List modules
$ phaser modules
# Display scan options
$ phaser scan --help
# Scan a target
$ phaser scan --aggressive kerkour.com
```


### With Docker

```shell
$ docker run -ti ghcr.io/skerkour/phaser phaser scan --aggressive kerkour.com
```

## License

See [`LICENSE.txt`](./LICENSE.txt).
