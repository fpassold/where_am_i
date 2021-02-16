# Project Where Am I

Project #3: Where Am I /src files.

Project associated with using a robot assembled in project 2, introducing it to a customized world (with some obstacles), extracting the map file (using pgm_map_creator plugin) and executing and testing the AMCL localization algorithm (ROS package).

Some notes:

* Fixed bugs related to subcribe laser dada sensor to AMCL node, related to the (incorrect) reference to topic `/laser/scan` (in `amcl.launch` and `costmap_common_params.yaml` file) that should be simple `/scan` as programmed (appears) in final lines of the `my_robot.gazebo` file;
* Varied some parameters (related to AMCL algorithm) in `costmap_common_params.yaml` file;
* extended laser sensor opening angle from -90 to +90 degrees to -120 to +120 degrees -- `my_robot.gazebo`.

Fernando Passold, 16 Feb 2021.
