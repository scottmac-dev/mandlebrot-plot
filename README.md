# Mandlebrot plot
This Rust program can be used to generate custom mandlebrot plots via the CLI terminal.

I created it while working through the Programming Rust text book and take no credit for the source code, it was created purely as a learning experience.

[Get The Book](https://www.oreilly.com/library/view/programming-rust-2nd/9781492052586/)
[About The Mandlebrot Plot Set](https://en.wikipedia.org/wiki/Mandelbrot_set)
[Install Rust](https://www.rust-lang.org/tools/install)

## Requirements
    - rustc
    - cargo

## Running the program
```bash 
cargo build --release # compile and build program with rustc
target/release/mandlebrot FILENAME PIXELS UPPERLEFT LOWERRIGHT
# Example/Recommended for a nice output
target/release/mandlebrot mandel.png 1000x750 -1.20,0.35 -1,0.20
```

## Change colour
To change between light and dark mode modify line 66 of main.rs
```bash 
Some(count) => 255 - count as u8 # Light-mode
Some(count) => 0 + count as u8 # Dark mode
```


