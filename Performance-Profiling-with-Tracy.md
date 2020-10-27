<img src="https://user-images.githubusercontent.com/1389729/97106613-832f0100-16cb-11eb-8452-267e406bceb9.png" width="640" height="480"/>

```
A real time, nanosecond resolution, remote telemetry, hybrid frame and sampling profiler for games and other applications.
```
**Tracy GitHub:** https://github.com/wolfpld/tracy

**Tracy Release v0.7.3:** https://github.com/wolfpld/tracy/releases/download/v0.7.3/Tracy-0.7.3.7z

**Tracy User Guide:** https://github.com/wolfpld/tracy/releases/download/v0.7.3/tracy.pdf

## Intro

We can't know how good/bad our performance is until we measure it.

`Tracy` is made up of two parts:
- The client - which you build into your program and will broadcast your performance information.
- The server - an external program (available in the Tracy Release) which will receive the information and allow you to analyze it. 

## Setup

Add `-DTRACY_ENABLE=ON` to your `CMake` configuration arguments. It will download and build the `Tracy` client into `topaz_game` for you.

1) Build `topaz_game` with `-DTRACY_ENABLE=ON`
2) Launch `Tracy.exe` from the Tracy Release
3) In Tracy, press "Connect". It will wait for data to be sent to it.
4) Launch `topaz_game` and watch the data stream in.