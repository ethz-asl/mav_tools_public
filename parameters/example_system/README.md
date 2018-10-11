**These parameters are examples only.**

Even if you have the exact same hardware setup as the platform they were created for you will need to regenerate all of them.

* **camchain.yaml** is generated via [Kalibr](https://github.com/ethz-asl/kalibr) and contains intrinsic and extrinsic camera-imu calibration information
* **rovio_filter.info** and **rovio_cam0.yaml** contain the parameters needed by rovio. The calibration parameters need in these are generated from the camchain.yaml.
* **nonlinear_mpc.yaml** and **disturbance_observer.yaml** contain parameters governing the use of the model predictive controller. They are generated from the system id flight plus hand tuning to fit your system.
* **px4_config.yaml** gives some parameters needed by mavros and the PX4. The thrust constant value is given via sysid, with the other parameters set depending on your setup.
* **example_radio_setup.otx** is an example of how our RC controller is configured using OpenTX
* **example_system/example_px4_parameters.params** contains the parameters loaded on the example platforms PX4 
