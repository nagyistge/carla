CARLA Design
============

> _This document is a work in progress and might be incomplete._

CARLA is composed by the following modules

  * Client side
    - Python client API: "PythonClient/carla"
  * Server side
    - CarlaUE4 Unreal Engine project: "Unreal/CarlaUE4"
    - Carla plugin for Unreal Engine: "Unreal/CarlaUE4/Plugins/Carla"
    - CarlaServer: "Util/CarlaServer"

Python client API
-----------------

The client API provides a Python module for communicating with the CARLA server.
In the folder "PythonClient", we provide several examples for scripting a CARLA
client using the "carla" module.

CarlaUE4 Unreal Engine project
------------------------------

The Unreal project "CarlaUE4" contains all the assets and scenes for generating
the CARLA binary. It uses the tools provided by the Carla plugin to assemble the
cities and behavior of the agents in the scene.

Carla plugin for Unreal Engine
------------------------------

The Carla plugin contains all the functionality of CARLA. We tried to keep this
functionality separated from the assets, so the functionality in this plugin can
be used as much as possible in any Unreal project.

It uses "CarlaServer" library for the networking communication.

CarlaServer
-----------

External library for the networking communications.

See ["CarlaServer"](carla_server.md) for implementation details.
