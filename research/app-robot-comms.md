# API Server solution for App-to-robot communications

**The Problem**: We cannot effectively communicate to the robot via the iOS app.

**Solution**: Create an API server that translates requests from the iOS app into valid ROS2 API calls to control the iRC3 robot.

## Why can't the iOS App control the iRobot Create 3?

The only library that was found that has ROS2 bindings that work on iOS is [one written for Objective-C](https://github.com/esteve/ros2_objc). Officially, and very obviously, this library is unmaintained and not usable for our project. We oiginally thought that [PythonKit](https://github.com/pvieito/PythonKit) could solve our issues by running python code under iOS, however this does not solve the issue of still needing the ROS2 middleware.

## The API Server

The solution that we came up with was to create our own API server that will take requests from the iOS app and translate them into ROS2 commands. This will allow us to remotely control the robot from the app without needing to use ROS2 bindings on the app directly.

This server could run on a [Raspberry Pi connected directly to the iRC3 robot](https://iroboteducation.github.io/create3_docs/hw/rpi_hookup/). This would mean that there are no additional pieces of hardware outside of the iRC3 chassis. This project would probably require a Pi anyway in order for WiFi scanning.
