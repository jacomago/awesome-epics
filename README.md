# Awesome [EPICS](https://epics-controls.org/)

The Experimental Physics and Industrial Control System (EPICS) is a set of software tools and applications used to develop and implement distributed control systems to operate devices such as particle accelerators, telescopes and other large experiments.

* [Main EPICS Links](#main-epics-links)
* [Base](#base)
    * [Editor Extensions](#editor-extensions)
    * [Network Protocols](#network-protocols)
        * [pvAccess](#pvaccess)
        * [Channel Access](#channel-access)
* [Modules](#modules)
* [Packaging](#packaging)
* [IOC Runners](#ioc-runners)
* [Applications](#applications)
* [Other Lists](#other-lists)

## Main EPICS Links

* [EPICS Tech Talk Mailing List](https://epics.anl.gov/tech-talk/) - The main forum for talking about EPICS and the other parts of the ecosystem.
* [EPICS Controls](https://epics-controls.org/) - The newer home for EPICS.
* [EPICS Argonne Home](https://epics.anl.gov/) - The older website hosted at Argonne National Laboratory.
* [EPICS Documentation](https://docs.epics-controls.org/en/latest/index.html)
* [EPICS Github Organization](https://github.com/epics-base)

## Base

* [EPICS Base](https://github.com/epics-base/epics-base) - EPICS is a set of Open Source software tools, libraries and applications developed collaboratively and used worldwide to create distributed soft real-time control systems for scientific instruments such as a particle accelerators, telescopes and other large scientific experiments.
* [EPICS Docs](https://github.com/epics-docs/epics-docs) - Documentation for EPICS Base.

### Editor Extensions

* [vscode](https://github.com/epics-extensions/vscode-epics) - VS Code colorization for EPICS database, templates and substitution files.
* [epics.nvim](https://github.com/epics-extensions/epics.nvim) - EPICS-related tools for Neovim including syntax highlighting and utilities.

### Network Protocols

#### pvAccess

pvAccess is a high-performance network communication protocol for signal monitoring and scientific data services interconnect.

* [pvAccess Specification](https://github.com/epics-base/pvAccessCPP/wiki/Protocol-Encoding)
* [Original C++ Implementation](https://github.com/epics-base/pvAccessCPP) _(archived)_
* [pvxs C++ Implementation](https://mdavidsaver.github.io/pvxs/index.html)
* [p4p](https://github.com/epics-base/p4p) - Python bindings for pvAccess, providing client and server APIs.
* [pvaPy](https://github.com/epics-base/pvaPy) - Python API for pvAccess with support for PvObject serialization and RPC services.
* [Original Java Implementation](https://github.com/epics-base/epicsCoreJava/tree/3a32ca5dbc2fd9db610c3d7c08e37600b9aa0b32/pvAccessJava#readme) _(archived)_
* [Phoebus Java Implementation](https://github.com/ControlSystemStudio/phoebus/tree/master/core/pva)

#### Channel Access

* [Channel Access Specification](https://docs.epics-controls.org/en/latest/specs/ca_protocol.html)
* [Java Implementation](https://github.com/epics-base/jca)
* [pyepics](https://github.com/pyepics/pyepics) - PyEpics is a Python interface to the EPICS Channel Access (CA) library for the EPICS control system.
* [cothread](https://github.com/DiamondLightSource/cothread) - Python library for asynchronous Channel Access using cooperative threading. _(site-Diamond)_
* [caproto](https://github.com/caproto/caproto) - Pure-Python Channel Access implementation (client and server) with a pluggable I/O model.
* [pcaspy](https://github.com/paulscherrerinstitute/pcaspy) - Portable Channel Access Server in Python for embedding CA servers in Python applications. _(site-PSI)_
* [aioca](https://github.com/DiamondLightSource/aioca) - Asynchronous Channel Access client for Python asyncio. _(site-Diamond)_
* [ophyd](https://github.com/bluesky/ophyd) - Hardware abstraction layer for EPICS and other control systems, part of the Bluesky ecosystem.

## Modules

* [asyn](https://github.com/epics-modules/asyn) - EPICS module for driver and device support.
* [StreamDevice](https://github.com/paulscherrerinstitute/StreamDevice) - EPICS Driver for message based I/O. _(site-PSI)_
* [recsync](https://github.com/ChannelFinder/recsync) - EPICS Record Synchronizor.
* [mca](https://github.com/epics-modules/mca) - EPICS support for multi-channel analyzers (MCA) and multi-channel scalers (MCS).
* [motor](https://github.com/epics-modules/motor) - EPICS motor record and device support for a wide range of motion controllers.
* [iocStats](https://github.com/epics-modules/iocStats) - IOC statistics and health monitoring records.
* [opcua](https://github.com/epics-modules/opcua) - EPICS device support for OPC UA servers.
* [areaDetector](https://github.com/areaDetector/ADCore) - Framework and core library for detector and camera integration.
* [PyDevice](https://github.com/klemenv/PyDevice) - Device support for writing IOC functionality directly in Python.
* [pyDevSup](https://github.com/epics-modules/pyDevSup) - Device support layer for implementing EPICS record processing in Python.
* [modbus](https://github.com/epics-modules/modbus) - EPICS support for Modbus TCP/IP and serial communication with PLCs and other devices.
* [ecmc](https://github.com/epics-modules/ecmc) - EPICS support for EtherCAT motion and generic I/O controllers.
* [autosave](https://github.com/epics-modules/autosave) - Saves and restores IOC PV values across restarts.
* [mrfioc2](https://github.com/epics-modules/mrfioc2) - EPICS driver for Micro Research Finland event-based timing system devices.
* [sequencer](https://github.com/epics-modules/sequencer) - State Notation Language (SNL) compiler and runtime sequencer for writing state machine programs in EPICS IOCs.
* [ether_ip](https://github.com/epics-modules/ether_ip) - EPICS device support for Allen-Bradley PLCs via the EtherIP protocol.
* [caPutLog](https://github.com/epics-modules/caPutLog) - Logs Channel Access put operations to iocLogServer for audit trails.
* [calc](https://github.com/epics-modules/calc) - synApps module providing sCalcout, swait, transform, and other calculation record types.
* [sscan](https://github.com/epics-modules/sscan) - Programmatically configures conditions and acquires data across positioner ranges; standard at experimental beamlines.
* [mqtt](https://github.com/epics-modules/mqtt) - Native EPICS support for the MQTT protocol, enabling integration with IoT brokers.
* [twincat-ads](https://github.com/epics-modules/twincat-ads) - EPICS device support for communicating with Beckhoff TwinCAT PLCs via the ADS protocol.
* [lua](https://github.com/epics-modules/lua) - Lua shell and scripting interfaces for EPICS IOCs.
* [devlib2](https://github.com/epics-modules/devlib2) - Portable helper library for PCIbus, MMIO, and VME64 CR/CSR hardware access; used by many hardware support modules.

## Packaging

* [e3](https://gitlab.esss.lu.se/e3/e3) - Allows for easily building EPICS modules directly from source and automagically resolves module dependencies, and allows for site-specific modifications to EPICS modules without needing to directly modify source trees. _(site-ESS)_
* [EPNix](https://epics-extensions.github.io/EPNix/nixos-25.11/) - EPNix (pronunciation: as if you are high on mushrooms) enables you to build, package, deploy IOCs and other EPICS-related software by using the Nix package manager.
* [EPICS Containers](https://github.com/epics-containers) - A collection of tools and documentation for building, deploying and managing containerized EPICS IOCs in a Kubernetes cluster.

## IOC Runners

* [procServ](https://github.com/ralphlange/procServ) - Process server: wraps an IOC (or any child process) with a telnet console and automatic restart.
* [pythonSoftIOC](https://github.com/DiamondLightSource/pythonSoftIOC) - Embed a fully functional EPICS IOC in a Python process. _(site-Diamond)_
* [systemd-softioc](https://github.com/NSLS2/systemd-softioc) - systemd service scripts for managing EPICS soft IOCs via procServ.
* [ibek](https://github.com/epics-containers/ibek) - IOC Builder for EPICS and Kubernetes: generates IOC startup scripts from YAML.

## Applications

* [Channel Finder](https://github.com/ChannelFinder/ChannelFinderService) - A RESTful directory service for a list of channels.
* [Archiver](https://github.com/archiver-appliance/epicsarchiverap) - This is an implementation of an archiver for EPICS control systems that aims to archive millions of PVs.
* [Alarm Service](https://github.com/ControlSystemStudio/phoebus/tree/master/app/alarm) - EPICS alarm handling system, part of the Phoebus suite.
* [Phoebus](https://github.com/ControlSystemStudio/phoebus) - A framework and set of tools to monitor and operate large scale control systems, such as the ones in the accelerator community.
* [PyDM](https://github.com/slaclab/pydm) - Python Display Manager: widget toolkit for building control system operator interfaces. _(site-SLAC)_
* [React-Automation-Studio](https://github.com/React-Automation-Studio/React-Automation-Studio) - Web-based EPICS operator interface platform built with React and Node.js.
* [VisualDCT](https://github.com/epics-extensions/VisualDCT) - Visual Database Configuration Tool: graphical editor for EPICS database files.
* [oac-tree](https://github.com/oac-tree/oac-tree-bundle) - Behavior-tree-based procedure sequencing framework for EPICS control systems.
* [ca-gateway](https://github.com/epics-extensions/ca-gateway) - Channel Access PV Gateway: bridges multiple CA subnets and enforces access security.
* [pvws](https://github.com/ornl-epics/pvws) - PV Web Socket: serves Channel Access and pvAccess PVs over WebSockets to browser clients.
* [epics2web](https://github.com/JeffersonLab/epics2web) - Web gateway that exposes EPICS CA PVs via a JSON WebSocket API.
* [weiss](https://github.com/weiss-controls/weiss) - Web EPICS Interface & Synoptic Studio: drag-and-drop tool for building EPICS web operator interfaces.
* [phoebusgen](https://github.com/als-epics/phoebusgen) - Python library for generating Phoebus OPI display files programmatically.
* [lewis](https://github.com/ISISComputingGroup/lewis) - Python framework for writing simulated hardware devices for testing EPICS IOC control systems.
* [cashark](https://github.com/mdavidsaver/cashark) - Wireshark dissector plugin for decoding EPICS Channel Access and pvAccess network traffic.
* [CALab](https://github.com/epics-extensions/CALab) - Channel Access client plugin for LabVIEW.
* [medm](https://github.com/epics-extensions/medm) - Motif Editor and Display Manager: a legacy X11/Motif display tool, still in use at many sites.
* [caQtDM](https://github.com/caqtdm/caqtdm) - Qt-based display manager with MEDM migration tools; runs on Linux, Windows, macOS, iOS, and Android.
* [StripTool](https://github.com/epics-extensions/StripTool) - Legacy strip-chart plotting tool for Channel Access PVs.
* [alh](https://github.com/epics-extensions/alh) - Alarm Handler: legacy GUI tool for monitoring and acknowledging EPICS alarms. Superseded by the Phoebus alarm system.
* [c2dataviewer](https://github.com/epics-extensions/c2dataviewer) - Python GUI front-end for visualizing AreaDetector and pvAccess image data.
* [archiverappliance-datasource](https://github.com/sasaki77/archiverappliance-datasource) - Grafana datasource plugin for querying EPICS Archiver Appliance data.
* [whatrecord](https://github.com/pcdshub/whatrecord) - IOC meta-information tool: parses EPICS databases, startup scripts, and snl programs.
* [epicsdbbuilder](https://github.com/DiamondLightSource/epicsdbbuilder) - Python library for programmatically building EPICS database files. _(site-Diamond)_
* [CS Studio](https://github.com/ControlSystemStudio/cs-studio) - Eclipse-based predecessor to Phoebus for monitoring and operating large scale control systems. Superseded by Phoebus. _(archived)_

## Other Lists

* [EPICS Extensions](https://epics.anl.gov/extensions/index.php) - The following list gives access to individual pages for most of the standard EPICS host tools and CA clients.
* [EPICS SoftSupport](https://epics-controls.org/resources-and-support/modules/soft-support/) - The following table contains an index of EPICS Soft Support modules available for use within IOCs.
