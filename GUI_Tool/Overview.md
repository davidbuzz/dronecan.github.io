---
weight: 0
permalink: /GUI_Tool/Overview/
---

# DroneCAN GUI Tool

{% include lightbox.html url="/GUI_Tool/figures/screenshot.png" title="DroneCAN GUI Tool" thumbnail="true" %}

{% include lightbox.html url="/GUI_Tool/figures/demo_sin_cos_setpoint.png" title="Using the embedded IPython console" thumbnail="true" %}

{% include lightbox.html url="/GUI_Tool/figures/demo_node_configuration.png" title="Remote node reconfiguration" thumbnail="true" %}

DroneCAN GUI Tool is a cross-platform free open source application for DroneCAN bus management and diagnostics.
It runs on Windows, Linux, and OSX.

* Real time monitoring of CAN bus and DroneCAN transfer dissection.
* Plotting values in real time.
* Remote node reconfiguration (`uavcan.protocol.param`).
* Firmware update on remote nodes.
* Python scripting from the embedded IPython console.
* Different CAN adapter backends supported:
  * SLCAN (aka LAWICEL) adapters, e.g. [Zubax Babel](https://zubax.com/products/babel).
  * Linux [SocketCAN](https://en.wikipedia.org/wiki/SocketCAN).

## Installation

### Windows

Download and install the latest MSI package from <https://firmware.ardupilot.org/Tools/CAN_GUI/>.

### Linux

Note that if you're using a USB SLCAN adapter, it may be necessary to
[configure serial port access permissions](https://kb.zubax.com/x/N4Ah).

#### Ubuntu, Mint, and other Debian-based distros


```bash

sudo apt-get install -y python3-pip python3-setuptools python3-wheel
sudo apt-get install -y python3-numpy python3-pyqt5 python3-pyqt5.qtsvg git-core
sudo pip3 install pydronecan
sudo pip3 install git+https://github.com/DroneCAN/gui_tool@master
```

#### Other distributions

Please refer to the README file in the source repository: <https://github.com/DroneCAN/gui_tool>.

### OSX

Please refer to the README file in the source repository: <https://github.com/DroneCAN/gui_tool>.

## Feedback

Direct your questions and feedback to the [discussion area](/Contact).

Pull requests and bug reports are welcome at the GitHub repository at <https://github.com/DroneCAN/gui_tool>.
