# Creating a Python package for ROS2

This is a quick doc to go over how to create a python package for use with ros2 command line

## Create the ROS2 package

The package first must be created/initialized as follows:

```
ros2 pkg create package_name --build-type ament_python
```

## Editing the package
Edit `setup.py` appropriately. Add any needed packages. Create the modules you want in the package under the package directory. This directory woulld be `package_name/package_name`. 

## Building

Run the following in the package root:

```
colcon build --symlink-install
```

## Sourcing
Source the `local_setup.sh` file in .bashrc

```
source /path/to/install/folder/local_setup.sh`
```

## Finishing up

Restart your terminal session and you should be able to run `ros2 run package_name module_name` assuming you set up the console scripts entrypoint correctly (check ros2 create3 examples for this)
