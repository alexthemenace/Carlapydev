CARLA Simulator
===============


[![carla.org](Docs/img/btn/web.png)](http://carla.org)
[![download](Docs/img/btn/download.png)](https://github.com/carla-simulator/carla/blob/master/Docs/download.md)
[![documentation](Docs/img/btn/docs.png)](http://carla.readthedocs.io)
[![forum](Docs/img/btn/forum.png)](https://github.com/carla-simulator/carla/discussions)
[![discord](Docs/img/btn/chat.png)](https://discord.gg/8kqACuC)

CARLA is an open-source simulator for autonomous driving research. CARLA has been developed from the ground up to support development, training, and
validation of autonomous driving systems. In addition to open-source code and protocols, CARLA provides open digital assets (urban layouts, buildings,
vehicles) that were created for this purpose and can be used freely. The simulation platform supports flexible specification of sensor suites and
environmental conditions.

[![CARLA Video](Docs/img/0_9_15_thumbnail.webp)](https://www.youtube.com/watch?v=q4V9GYjA1pE )

### Download CARLA

Linux:
* [**Get CARLA overnight build**](https://tiny.carla.org/carla-latest-linux)
* [**Get AdditionalMaps overnight build**](https://tiny.carla.org/additional-maps-latest-linux)

Windows:
* [**Get CARLA overnight build**](https://tiny.carla.org/carla-latest-windows)
* [**Get AdditionalMaps overnight build**](https://tiny.carla.org/additional-maps-latest-windows)

### Recommended system

* Intel i7 gen 9th - 11th / Intel i9 gen 9th - 11th / AMD ryzen 7 / AMD ryzen 9
* +32 GB RAM memory
* NVIDIA RTX 3070 / NVIDIA RTX 3080 / NVIDIA RTX 4090
* Ubuntu 20.04



**Like what you see? Star us on GitHub to support the project!**


```
@inproceedings{Dosovitskiy17,
  title = {{CARLA}: {An} Open Urban Driving Simulator},
  author = {Alexey Dosovitskiy and German Ros and Felipe Codevilla and Antonio Lopez and Vladlen Koltun},
  booktitle = {Proceedings of the 1st Annual Conference on Robot Learning},
  pages = {1--16},
  year = {2017}
}
```

Building CARLA
--------------

Clone this repository locally from GitHub:

```sh
git clone https://github.com/Carlapydev .
```

Also, clone the [CARLA fork of the Unreal Engine](https://github.com/CarlaUnreal/UnrealEngine) into an appropriate location:

```sh
git clone --depth 1 -b carla https://github.com/CarlaUnreal/UnrealEngine.git .
```

Once you have cloned the repositories, follow the instructions for [building in Linux][buildlinuxlink] or [building in Windows][buildwindowslink].

[buildlinuxlink]: https://carla.readthedocs.io/en/latest/build_linux/
[buildwindowslink]: https://carla.readthedocs.io/en/latest/build_windows/

Contributing
------------

Please take a look at our [Contribution guidelines][contriblink].

[contriblink]: https://carla.readthedocs.io/en/latest/cont_contribution_guidelines/



CARLA uses three dependencies as part of the SUMO integration:
- [PROJ](https://proj.org/), a generic coordinate transformation software which uses the [X/MIT open source license](https://proj.org/about.html#license).
- [SQLite](https://www.sqlite.org), part of the PROJ dependencies, which is [in the public domain](https://www.sqlite.org/purchase/license).
- [Xerces-C](https://xerces.apache.org/xerces-c/), a validating XML parser, which is made available under the [Apache Software License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).

CARLA uses one dependency as part of the Chrono integration:
- [Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page), a C++ template library for linear algebra which uses the [MPL2 license](https://www.mozilla.org/en-US/MPL/2.0/).

CARLA uses the Autodesk FBX SDK for converting FBX to OBJ in the import process of maps. This step is optional, and the SDK is located [here](https://www.autodesk.com/developer-network/platform-technologies/fbx-sdk-2020-0)

This software contains Autodesk® FBX® code developed by Autodesk, Inc. Copyright 2020 Autodesk, Inc. All rights, reserved. Such code is provided "as is" and Autodesk, Inc. disclaims any and all warranties, whether express or implied, including without limitation the implied warranties of merchantability, fitness for a particular purpose or non-infringement of third party rights. In no event shall Autodesk, Inc. be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of such code."
