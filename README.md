# Floodlight_multicontroller
This is a floodlight controller with multi-controller capabilities based on our CIDC interface.
The Communication Interface for Distributed Control-plane (CIDC) is composed of four basic components: Consumer (listens for remote changes),
Producer(shares local changes to remote consumers), DataUpdater (updates the network state), and DataCollector(collects local changes). These components are full connected and communicate with the core components
of the controller. The behavior of these modules will depend on the configuration modes (Notification, Service, Full). These modes are freely configurable on the config file. 

Each controller plays the rule of a Consumer for external events and a Producer for local events. Their main goal is to exchange useful message between other controllers. 

To read more about this project, read the full paper here https://www.researchgate.net/publication/308856869_An_East-West_interface_for_distributed_SDN_control_plane_Implementation_and_evaluation?ev=prf_high
