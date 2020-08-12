# mediapipe sample project
This is a sample repository to setup a project that depends on mediapipe (v0.7.8).
The main program is just the same as [Hello World! on Desktop](https://google.github.io/mediapipe/getting_started/hello_world_desktop.html) code.

## Installation
Please follow the [mediapipe official installation guide](https://google.github.io/mediapipe/getting_started/install.html) and ensure that you can run the official Hello World sample on your desktop.

## Build & Run
```sh
git clone https://github.com/homuler/mediapipe-sample-project.git
cd mediapipe-sample-project

# Build
bazel build -c opt --define MEDIAPIPE_DISABLE_GPU=1 //mediapipe_sample:hello_world

# Run
GLOG_logtostderr=1 bazel run -c opt --define MEDIAPIPE_DISABLE_GPU=1 //mediapipe_sample:hello_world
```

## LICENSE
The main program (hello_world.cc) is distributed under [Apache License 2.0](https://github.com/homuler/mediapipe-sample-project/blob/master/LICENSE).
Other parts are distributed under [UNLICENSE](https://github.com/homuler/mediapipe-sample-project/blob/master/UNLICENSE).
