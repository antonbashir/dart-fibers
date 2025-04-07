# Dart Fiber [EXPERIMENTAL]

Dart Fibers is a patched dart-sdk which allows you to use coroutine mechanism in the Dart language. 

## How to ?

To use coroutines you need to compile Dart VM from this [branch](https://github.com/antonbashir/dart/pull/3).

Then you need to compile `main.dart` to `main.exe` with command `dart compile exe main.dart` 

Now run `main.exe`:

```
before start
main: entry
child: entry
main: after child transfer
main -> child -> main -> child
after start
```

![](fibers.gif)

## What is next ?

* Implement JIT mode
* Implement other architectures
* Implement channels
* Implement FFI
* Implement `async`
* Optimize
* Add more tests and benchmarks
* Support `JS` and `WASM` ?
