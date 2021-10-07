# usb_camera_ros
ROS Package that contains launch files and seetings to interface USB (UVC) cameras with ROS
# Dependencies
* **libuvc_camera**: `apt install -y ros-melodic-libuvc-camera`

# How to run?
* You can check the supported formats/frame rates of your camera using the command `v4l2-ctl --list-formats-ext -d /dev/video2`. `/dev/video2` might be different for your camera.
* Adjust the camera settings in `usb_camera_ros/config/cam_settings.yaml` according to your camera
* Run the `usb_cam.launch` file
```bash
roslaunch usb_camera_ros usb_camera.launch config_file:=/path/to/cam_settings.yaml
```
