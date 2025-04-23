# Mini Async Runtime

Mini Async Runtime is a lightweight and minimal implementation of an asynchronous runtime in Rust. It provides basic functionality for running asynchronous tasks, including task spawning, sleeping, and yielding.

## Features

- **Task Spawning**: Spawn asynchronous tasks and manage their execution.
- **Sleep Functionality**: Pause tasks for a specified duration using a custom timer.
- **Yielding**: Yield control back to the runtime to allow other tasks to execute.
- **Custom Runtime**: A simple runtime implementation with a task queue and waker mechanism.
- **Macros**: Includes procedural macros for simplifying async runtime usage.

## Project Structure

- `src/`: Contains the main runtime implementation and utility functions.
  - `components.rs`: Core components like `MiniRuntime`, `Task`, `Timer`, and `Sleep`.
  - `runtime.rs`: The runtime logic for task scheduling and execution.
  - `runtime_storage.rs`: Thread-local storage for the task queue.
  - `funtions.rs`: Helper functions like `spawn`, `sleep`, and `yield_now`.
  - `main.rs`: Example usage of the runtime.
- `minimal-async-macros/`: Contains procedural macros for extending runtime functionality.
- `Dockerfile`: Docker configuration for building and running the project.
- `.github/workflows/`: GitHub Actions workflow for building and pushing Docker images.

## Usage

### Running the Example

To run the example tasks defined in `src/main.rs`, use the following command:

```sh
cargo run
```
