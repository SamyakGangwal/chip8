
# CHIP-8 Emulator in Rust

Welcome to my implementation of a **CHIP-8 emulator** built using **Rust** and **SDL2**. This project is part of my journey into learning more about **computer architecture** and understanding the inner workings of emulation. The emulator faithfully replicates the CHIP-8 system, a simple, interpreted programming language popular in the 1970s, and allows you to run CHIP-8 programs, including classic games like Pong, Space Invaders, and more!

## Features

- **Core Emulation**: Accurate CHIP-8 instruction set implementation
- **Graphics**: Rendering via SDL2, replicating the original 64x32 pixel monochrome display
- **Input Handling**: Full support for CHIP-8 keypad mapping
- **Sound**: Beeper functionality (work in progress)
- **Double Buffering**: Currently working on reducing flickering with double buffering

## How to Build and Run

### Prerequisites

- **Rust** (latest stable version)
- **SDL2** development libraries

#### Linux
On Linux, you can install SDL2 via:
```bash
sudo apt-get install libsdl2-dev
```

#### macOS
On macOS, use:
```bash
brew install sdl2
```

#### Windows
On Windows, you will need to:

1. Install [Visual Studio](https://visualstudio.microsoft.com/) with the C++ build tools.
2. Install Rust using [rustup](https://rustup.rs/).
3. Download and install the [SDL2 development libraries for MinGW](https://www.libsdl.org/download-2.0.php). Make sure to place the `SDL2.dll` file in your project directory or system PATH.

### Build

Once you have the dependencies set up, clone the repository and build the project using Cargo:

```bash
git clone https://github.com/SamyakGangwal/chip8.git
cd chip8
cargo build --release
```

### Run

To run the emulator with a CHIP-8 ROM file:

```bash
cargo run --release path/to/your/rom.ch8
```

You can find some popular CHIP-8 ROMs online to try out with the emulator.

## Key Bindings

The CHIP-8 uses a hexadecimal keypad (0-9, A-F). The emulator maps these keys as follows:

| CHIP-8 Key | Mapped Key |
|------------|------------|
| 1          | 1          |
| 2          | 2          |
| 3          | 3          |
| C          | 4          |
| 4          | Q          |
| 5          | W          |
| 6          | E          |
| D          | R          |
| 7          | A          |
| 8          | S          |
| 9          | D          |
| E          | F          |
| A          | Z          |
| 0          | X          |
| B          | C          |
| F          | V          |

## Learning Journey

This project is part of my broader effort to dive deeper into **computer architecture** and the fundamental concepts behind how systems operate at a low level. Through building this emulator, I’ve gained insight into:

- **Opcode decoding and execution**
- **Memory management in constrained systems**
- **Input/output handling in low-level environments**
- **Rendering graphics with minimal resources**

## Shoutout

A huge shoutout to [@aquova](https://github.com/aquova) for their excellent tutorials and resources on CHIP-8 emulation! Their work has been a tremendous help in understanding the intricacies of CHIP-8 and emulation in general.

## To-Do / Future Enhancements

- **Sound support**: Implementing a beeper for sound functionality.
- **Improved rendering**: Fine-tuning double buffering to eliminate flickering issues.
- **Testing and Debugging**: More robust testing with additional CHIP-8 programs and games.

## Contributing

Feel free to open issues or contribute to the project. Any improvements or suggestions are welcome as I continue to learn and improve this emulator.

---

By the end of this project, I hope to have a more comprehensive understanding of how emulators work and gain further skills in Rust and systems programming. Stay tuned for updates!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
