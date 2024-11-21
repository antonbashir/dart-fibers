# Dart Fiber [EXPERIMENTAL]

Dart Fibers is a patched dart-sdk which allows you to use coroutine mechanism in the Dart language. 

## How to ?

To use coroutines you need to get compiled Dart VM from this [branch](https://github.com/antonbashir/dart/pull/2).
Then you could just build `main.dart` to `main.exe` by `dart compile exe main.dart` and run `main.exe`.
You should see the results:

```
before start
main: entry
child: entry
main: after child transfer
main -> child -> main -> child
after start
```

![](download.gif)

## What is next ?

* I'm going to support JIT mode (complicated)
* I'm going to support sync and async fibers (already working but need to add API)
* Tests and Benches
* JS ? Not sure.
* Upstream ? Maybe.
