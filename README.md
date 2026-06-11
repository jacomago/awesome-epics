# Awesome EPICS [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

The Experimental Physics and Industrial Control System (EPICS) is a set of software tools and applications used to develop and implement distributed control systems to operate devices such as particle accelerators, telescopes and other large experiments.

## Contents

- [Main EPICS Links](#main-epics-links)
- [Base](#base)
  - [Editor Extensions](#editor-extensions)
  - [Network Protocols](#network-protocols)
- [Modules](#modules)
  - [Driver Infrastructure](#driver-infrastructure)
  - [Motion & Industrial](#motion--industrial)
  - [Detectors & DAQ](#detectors--daq)
  - [Utilities](#utilities)
  - [Scripting](#scripting)
- [Deployment](#deployment)
  - [Build & Packaging](#build--packaging)
  - [IOC Templating & Generation](#ioc-templating--generation)
  - [Process Management & Runtime](#process-management--runtime)
- [Applications](#applications)
  - [Operator Interfaces](#operator-interfaces)
  - [Web & Gateways](#web--gateways)
  - [Archiving](#archiving)
  - [Directory & Metadata Services](#directory--metadata-services)
  - [Alarms](#alarms)
  - [Logging](#logging)
  - [IOC & Database Tools](#ioc--database-tools)
  - [Simulators & Test IOCs](#simulators--test-iocs)
  - [Diagnostics & Network Analysis](#diagnostics--network-analysis)
- [Tutorials & Training](#tutorials--training)
- [Other Lists](#other-lists)

## Main EPICS Links

- [EPICS Tech Talk Mailing List](https://epics.anl.gov/tech-talk/) - The main forum for talking about EPICS and the other parts of the ecosystem.
- [EPICS Controls](https://epics-controls.org/) - The newer home for EPICS.
- [EPICS Argonne Home](https://epics.anl.gov/) - The older website hosted at Argonne National Laboratory.
- [EPICS Documentation](https://docs.epics-controls.org/en/latest/index.html) - The official EPICS documentation site, covering Base, modules, and the wider ecosystem.
- [EPICS GitHub Organization](https://github.com/epics-base) - The epics-base GitHub organization hosting EPICS Base and core repositories.

## Base

- [EPICS Base](https://github.com/epics-base/epics-base) - EPICS is a set of Open Source software tools, libraries and applications developed collaboratively and used worldwide to create distributed soft real-time control systems for scientific instruments such as a particle accelerators, telescopes and other large scientific experiments.
- [EPICS Docs](https://github.com/epics-docs/epics-docs) - Documentation for EPICS Base.

### Editor Extensions

- [VSCode EPICS](https://github.com/epics-extensions/vscode-epics) - VS Code colorization for EPICS database, templates and substitution files.
- [epics.nvim](https://github.com/epics-extensions/epics.nvim) - EPICS-related tools for Neovim including syntax highlighting and utilities.
- [tree-sitter-epics](https://github.com/epics-extensions/tree-sitter-epics) - Parsers for EPICS DSL file types: .db, .template, .substitutions, .proto, and .st SNL files.
- [EPICS IDE (Eclipse)](https://epics.anl.gov/eclipse/plugins/epicsIde/) - Eclipse plug-in for EPICS development with project wizards and IOC management.

### Network Protocols

#### pvAccess

pvAccess is a high-performance network communication protocol for signal monitoring and scientific data services interconnect.

- [pvAccess Specification](https://docs.epics-controls.org/en/latest/pv-access/protocol.html) - The official specification of the pvAccess network protocol.
- [pvxs C++ Implementation](https://mdavidsaver.github.io/pvxs/index.html) - Modern C++11 library implementing pvAccess and Channel Access, with Python bindings (p4p).
- [Original C++ Implementation](https://github.com/epics-base/pvAccessCPP) - The original C++ pvAccess library. Archived.
- [p4p](https://github.com/epics-base/p4p) - Python bindings for pvAccess with client, server, and gateway (pvAgw) APIs.
- [pvaPy](https://github.com/epics-base/pvaPy) - Python API for pvAccess with support for PvObject serialization and RPC services.
- [Phoebus Java Implementation](https://github.com/ControlSystemStudio/phoebus/tree/master/core/pva) - The Java pvAccess implementation maintained within the Phoebus core.
- [Original Java Implementation](https://github.com/epics-base/epicsCoreJava/tree/3a32ca5dbc2fd9db610c3d7c08e37600b9aa0b32/pvAccessJava#readme) - The original Java pvAccess library in epicsCoreJava. Archived.
- [pva2pva](https://github.com/epics-base/pva2pva) - PVAccess gateway/proxy for bridging pvAccess networks; superseded by p4p.gw. Archived.
- [spvirit](https://github.com/ISISNeutronMuon/spvirit) - Complete pvAccess protocol suite in Rust (codec, client, server, NT types, Python bindings) (ISIS).
- [pvxs-sys](https://github.com/ctrl-sys-ui/pvxs-sys) - Low-level Rust FFI bindings for the pvxs C++ pvAccess library.

#### Channel Access

- [Channel Access Specification](https://docs.epics-controls.org/en/latest/specs/ca_protocol.html) - The official specification of the Channel Access network protocol.
- [Java Implementation](https://github.com/epics-base/jca) - Java Channel Access (JCA) client and server library.
- [pyepics](https://github.com/pyepics/pyepics) - Python interface to the EPICS Channel Access (CA) library for the EPICS control system.
- [caproto](https://github.com/caproto/caproto) - Pure-Python Channel Access implementation (client and server) with a pluggable I/O model.
- [pcaspy](https://github.com/paulscherrerinstitute/pcaspy) - Portable Channel Access Server in Python for embedding CA servers in Python applications (PSI).
- [cothread](https://github.com/DiamondLightSource/cothread) - Python library for asynchronous Channel Access using cooperative threading (Diamond Light Source).
- [aioca](https://github.com/DiamondLightSource/aioca) - Asynchronous Channel Access client for Python asyncio (Diamond Light Source).
- [ophyd](https://github.com/bluesky/ophyd) - Hardware abstraction layer for EPICS and other control systems, part of the Bluesky ecosystem.
- [NetChannelAccess](https://github.com/paulscherrerinstitute/NetChannelAccess) - Pure C#/.NET implementation of the Channel Access protocol (client and server) (PSI).
- [epicars](https://github.com/ndevenish/epicars) - Standalone pure-Rust Channel Access protocol client.
- [epics-ca](https://gitlab.com/agerasev/epics-ca) - Rust client library for Channel Access.
- [ca-nameserver](https://github.com/epics-extensions/ca-nameserver) - Channel Access PV name server: lets clients discover PVs without flooding every subnet.
- [cacm](https://github.com/anjohnson/cacm) - Channel Access Client Monitor: command-line CA monitoring tool.
- [caTools](https://github.com/dirk-zimoch/caTools) - PSI's enhanced Channel Access command-line tools (caget, caput, camonitor, cawait, and more) (PSI).

#### Other Language Bindings

Channel Access client interfaces for languages and environments beyond Python.

- [matlab_ca](https://github.com/epics-extensions/matlab_ca) - MATLAB Channel Access client providing MCAGET/MCAPUT/MCAMON functions.
- [labCA](https://github.com/till-s/epics-labca) - EPICS Channel Access interface for MATLAB and Scilab.
- [CALab](https://github.com/epics-extensions/CALab) - Channel Access client plugin for LabVIEW.

## Modules

### Driver Infrastructure

- [asyn](https://github.com/epics-modules/asyn) - EPICS module for driver and device support.
- [StreamDevice](https://github.com/paulscherrerinstitute/StreamDevice) - EPICS Driver for message based I/O (PSI).
- [devlib2](https://github.com/epics-modules/devlib2) - Portable helper library for PCIbus, MMIO, and VME64 CR/CSR hardware access; used by many hardware support modules.
- [regdev](https://github.com/paulscherrerinstitute/regdev) - Generic EPICS register-device support framework for memory-mapped and register-based hardware (PSI).
- [mmap](https://github.com/paulscherrerinstitute/mmap) - regDev driver for VME and file-based memory maps (PSI).
- [epics-open62541](https://github.com/KIT-IBPT/epics-open62541) - EPICS device support acting as an OPC UA client via the open62541 library (KIT).
- [asynPythonDriver](https://github.com/paulscherrerinstitute/asynPythonDriver) - Write an asynPortDriver entirely in Python (PSI).
- [pscdrv](https://github.com/mdavidsaver/pscdrv) - Portable Streaming Controller driver: EPICS device support for streaming socket-based hardware controllers.
- [linStat](https://github.com/mdavidsaver/linStat) - EPICS driver serving Linux system- and process-level statistics as PVs.
- [i2cDev](https://github.com/paulscherrerinstitute/i2cDev) - EPICS support and a simple API for I2C devices on Linux (PSI).

### Motion & Industrial

- [motor](https://github.com/epics-modules/motor) - EPICS motor record and device support for a wide range of motion controllers.
- [ecmc](https://github.com/epics-modules/ecmc) - EPICS support for EtherCAT motion and generic I/O controllers.
- [ecmccfg](https://github.com/paulscherrerinstitute/ecmccfg) - Configuration and deployment scripts for the EtherCAT Motion Controller (ecmc) (PSI).
- [ecat2](https://github.com/paulscherrerinstitute/ecat2) - PSI EtherCAT driver for EPICS (PSI).
- [modbus](https://github.com/epics-modules/modbus) - EPICS support for Modbus TCP/IP and serial communication with PLCs and other devices.
- [s7plc](https://github.com/paulscherrerinstitute/s7plc) - EPICS driver for communication with Siemens S7 PLCs (PSI).
- [ether_ip](https://github.com/epics-modules/ether_ip) - EPICS device support for Allen-Bradley PLCs via the EtherIP protocol.
- [directNetAsyn](https://github.com/anjohnson/directNetAsyn) - EPICS device support for Automation Direct (Koyo) PLCs over an Asyn serial connection.
- [twincat-ads](https://github.com/epics-modules/twincat-ads) - EPICS device support for communicating with Beckhoff TwinCAT PLCs via the ADS protocol.
- [opcua](https://github.com/epics-modules/opcua) - EPICS device support for OPC UA servers.
- [epics-SMC9300](https://github.com/KIT-IBPT/epics-SMC9300) - EPICS device support for the Huber SMC 9300 motor controller (KIT).
- [epics-DeltaPS](https://github.com/KIT-IBPT/epics-DeltaPS) - EPICS device support for Delta SM3300 series power supplies (KIT).
- [isara-arm](https://github.com/mdavidsaver/isara-arm) - EPICS driver for the ISARA sample-mounting robot.

### Detectors & DAQ

- [areaDetector](https://github.com/areaDetector/ADCore) - Framework and core library for detector and camera integration.
- [ndwarp](https://github.com/mdavidsaver/ndwarp) - NDPluginWarp: areaDetector plugin for image spatial-distortion correction / warping.
- [slsDetector](https://github.com/paulscherrerinstitute/slsDetector) - areaDetector driver for SLS Detector Group detectors (Eiger, Jungfrau, Mythen) (PSI).
- [ADZMQ](https://github.com/paulscherrerinstitute/ADZMQ) - ZMQ ADDriver and NDPlugin for streaming areaDetector image data over ZeroMQ (PSI).
- [cam_server](https://github.com/paulscherrerinstitute/cam_server) - Camera server that converts EPICS-enabled cameras into bsread image streams (PSI).
- [mca](https://github.com/epics-modules/mca) - EPICS support for multi-channel analyzers (MCA) and multi-channel scalers (MCS).
- [sscan](https://github.com/epics-modules/sscan) - Programmatically configures conditions and acquires data across positioner ranges; standard at experimental beamlines.
- [calc](https://github.com/epics-modules/calc) - synApps module providing sCalcout, swait, transform, and other calculation record types.
- [mrfioc2](https://github.com/epics-modules/mrfioc2) - EPICS driver for Micro Research Finland event-based timing system devices.
- [epics-picoharp](https://github.com/KIT-IBPT/epics-picoharp) - EPICS driver for PicoQuant PicoHarp 300 time-correlated photon counter (KIT).

### Utilities

- [sequencer](https://github.com/epics-modules/sequencer) - State Notation Language (SNL) compiler and runtime sequencer for writing state machine programs in EPICS IOCs.
- [autosave](https://github.com/epics-modules/autosave) - Saves and restores IOC PV values across restarts.
- [caPutLog](https://github.com/epics-modules/caPutLog) - Logs Channel Access put operations to iocLogServer for audit trails.
- [iocStats](https://github.com/epics-modules/iocStats) - IOC statistics and health monitoring records.
- [mqtt](https://github.com/epics-modules/mqtt) - Native EPICS support for the MQTT protocol, enabling integration with IoT brokers.
- [epics-execute](https://github.com/KIT-IBPT/epics-execute) - EPICS device support for executing arbitrary shell scripts from an IOC (KIT).
- [IocshDeclWrap](https://github.com/paulscherrerinstitute/IocshDeclWrap) - C++ templates for easily wrapping user functions as EPICS IOC-shell commands (PSI).
- [iocsh_utilities](https://github.com/paulscherrerinstitute/iocsh_utilities) - Assorted EPICS IOC-shell utility commands (PSI).

### Scripting

- [PyDevice](https://github.com/klemenv/PyDevice) - Device support for writing IOC functionality directly in Python.
- [pyDevSup](https://github.com/epics-modules/pyDevSup) - Device support layer for implementing EPICS record processing in Python.
- [lua](https://github.com/epics-modules/lua) - Shell and scripting interfaces for EPICS IOCs using the Lua language.

## Deployment

### Build & Packaging

- [e3](https://gitlab.esss.lu.se/e3/e3) - Allows for easily building EPICS modules directly from source and automagically resolves module dependencies, and allows for site-specific modifications to EPICS modules without needing to directly modify source trees (ESS).
- [EPNix](https://epics-extensions.github.io/EPNix/nixos-25.11/) - Build, package, and deploy IOCs and other EPICS-related software using the Nix package manager.
- [EPICS Containers](https://github.com/epics-containers) - A collection of tools and documentation for building, deploying and managing containerized EPICS IOCs in a Kubernetes cluster.
- [EPICS on conda-forge](https://github.com/conda-forge/epics-base-feedstock) - conda-forge feedstock for the `epics-base` package; installs EPICS Base and tools (medm, striptool, probe, alh, extensions) via conda.
- [require](https://github.com/paulscherrerinstitute/require) - Runtime loader for EPICS IOCs that dynamically loads versioned support modules; the core of PSI's `driver.makefile` build system (PSI).
- [makeUtils](https://github.com/paulscherrerinstitute/makeUtils) - Extensions for PSI's `driver.makefile`, used together with require (PSI).
- [EPICS-env](https://github.com/jeonghanlee/EPICS-env) - Reproducible EPICS Base + modules build/configuration environment.
- [EPICS-env-distribution](https://github.com/jeonghanlee/EPICS-env-distribution) - Pre-built binary distribution of the EPICS-env environment.

### IOC Templating & Generation

- [ibek](https://github.com/epics-containers/ibek) - IOC Builder for EPICS and Kubernetes: generates IOC startup scripts from YAML.
- [EPICS-IOC-template-tools](https://github.com/jeonghanlee/EPICS-IOC-template-tools) - ALS-U EPICS IOC template generator (ALS-U).

### Process Management & Runtime

- [procServ](https://github.com/ralphlange/procServ) - Process server: wraps an IOC (or any child process) with a telnet console and automatic restart.
- [pythonSoftIOC](https://github.com/DiamondLightSource/pythonSoftIOC) - Embed a fully functional EPICS IOC in a Python process (Diamond Light Source).
- [systemd-softioc](https://github.com/NSLS2/systemd-softioc) - Systemd service scripts for managing EPICS soft IOCs via procServ.
- [iocmanager](https://github.com/pcdshub/iocmanager) - PyQt5 GUI for configuring and monitoring EPICS IOC processes across a facility (SLAC/PCDS).
- [epics-ioc-runner](https://github.com/jeonghanlee/epics-ioc-runner) - CLI tool for managing (start/stop/status) EPICS IOC processes.
- [epics_NIOCs](https://github.com/jeonghanlee/epics_NIOCs) - Setup tool for running multiple IOCs on a single Linux host.

## Applications

### Operator Interfaces

- [Phoebus](https://github.com/ControlSystemStudio/phoebus) - A framework and set of tools to monitor and operate large scale control systems, such as the ones in the accelerator community.
- [caQtDM](https://github.com/caqtdm/caqtdm) - Qt-based display manager with MEDM migration tools; runs on Linux, Windows, macOS, iOS, and Android.
- [PyDM](https://github.com/slaclab/pydm) - Python Display Manager: widget toolkit for building control system operator interfaces (SLAC).
- [React-Automation-Studio](https://github.com/React-Automation-Studio/React-Automation-Studio) - Web-based EPICS operator interface platform built with React and Node.js.
- [weiss](https://github.com/weiss-controls/weiss) - Web EPICS Interface & Synoptic Studio: drag-and-drop tool for building EPICS web operator interfaces.
- [DBWR](https://github.com/ornl-epics/dbwr) - Display Builder Web Runtime: renders Phoebus .bob OPI files in any browser with no client installation (ORNL).
- [medm](https://github.com/epics-extensions/medm) - Motif Editor and Display Manager: a legacy X11/Motif display tool, still in use at many sites.
- [EDM](https://github.com/slac-epics/edm) - Extensible Display Manager: X11/Motif-based interactive GUI builder for EPICS operator interfaces, widely used at facilities (SLAC).
- [StripTool](https://github.com/epics-extensions/StripTool) - Legacy strip-chart plotting tool for Channel Access PVs.
- [jstriptool](https://github.com/paulscherrerinstitute/jstriptool) - Java reimplementation of StripTool for strip-chart plotting of Channel Access PVs (PSI).
- [PShell](https://github.com/paulscherrerinstitute/pshell) - Java/Python scientific scripting workbench and GUI for controlling EPICS-based experiments (PSI).
- [CS Studio](https://github.com/ControlSystemStudio/cs-studio) - Eclipse-based predecessor to Phoebus for monitoring and operating large scale control systems. Superseded by Phoebus. Archived.

### Web & Gateways

- [ca-gateway](https://github.com/epics-extensions/ca-gateway) - Channel Access PV Gateway: bridges multiple CA subnets and enforces access security.
- [pvws](https://github.com/ornl-epics/pvws) - PV Web Socket: serves Channel Access and pvAccess PVs over WebSockets to browser clients.
- [pvws-springboot](https://github.com/ControlSystemStudio/pvws-springboot) - Spring Boot reimplementation of the pvws PV WebSocket server.
- [epics2web](https://github.com/JeffersonLab/epics2web) - Web gateway that exposes EPICS CA PVs via a JSON WebSocket API.
- [wica-http](https://github.com/paulscherrerinstitute/wica-http) - HTTP streaming service providing real-time browser access to live EPICS control-system data (PSI).

### Archiving

- [Archiver](https://github.com/archiver-appliance/epicsarchiverap) - This is an implementation of an archiver for EPICS control systems that aims to archive millions of PVs.
- [Phoebus Archive Engine](https://github.com/ControlSystemStudio/phoebus/tree/master/services/archive-engine) - EPICS archive engine in Phoebus: stores PV history to RDB (MySQL, PostgreSQL, TimescaleDB).
- [epics-archiver (Rust)](https://github.com/physwkim/archiver-rs) - Rust port of the EPICS Archiver Appliance with CA/pvAccess ingestion and PlainPB storage.
- [ChannelArchiver](https://github.com/epics-extensions/ChannelArchiver) - Legacy EPICS Channel Archiver predating Archiver Appliance; minimal maintenance. Archived.
- [archiverappliance-datasource](https://github.com/sasaki77/archiverappliance-datasource) - Grafana datasource plugin for querying EPICS Archiver Appliance data.
- [epicsarchiver-retrieval-client](https://github.com/archiver-appliance/epicsarchiver-retrieval-client) - Official Python library and CLI for retrieving data from the EPICS Archiver Appliance.
- [epicsarchiverap_pbrawclient](https://github.com/archiver-appliance/epicsarchiverap_pbrawclient) - Official Java client for the Archiver Appliance binary (PB raw) retrieval protocol.
- [epicsarchiver-mgmt-client](https://github.com/archiver-appliance/epicsarchiver-mgmt-client) - Official Python library and CLI for the Archiver Appliance management (mgmt) interface.
- [archapp](https://github.com/pcdshub/archapp) - Python client for Archiver Appliance with Pandas/xarray support (SLAC/PCDS).
- [aaclient](https://github.com/mdavidsaver/aaclient) - Python client for the EPICS Archiver Appliance.
- [eapy](https://github.com/epics-extensions/eapy) - Python interface to the ChannelArchiver V4 data access layer.
- [epicsarchiverap-env](https://github.com/jeonghanlee/epicsarchiverap-env) - Configuration/build environment for deploying the EPICS Archiver Appliance.

### Directory & Metadata Services

- [Channel Finder](https://github.com/ChannelFinder/ChannelFinderService) - A RESTful directory service for a list of channels.
- [pvinfo](https://github.com/ChannelFinder/pvinfo) - Web interface to ChannelFinder with integrations to other high-level control applications.
- [pyCFClient](https://github.com/ChannelFinder/pyCFClient) - Python client library for the ChannelFinder directory service.
- [recsync](https://github.com/ChannelFinder/recsync) - EPICS Record Synchronizor.
- [recsync-rs](https://github.com/ChannelFinder/recsync-rs) - Rust implementation of the RecSync protocol with Python bindings.
- [cfNameserver](https://github.com/ChannelFinder/cfNameserver) - pvAccess PV name server that resolves PVs using ChannelFinder and recsync information.

### Alarms

- [Alarm Service](https://github.com/ControlSystemStudio/phoebus/tree/master/app/alarm) - EPICS alarm handling system, part of the Phoebus suite.
- [alarm-logger](https://github.com/ControlSystemStudio/phoebus/tree/master/services/alarm-logger) - Phoebus service that archives alarm events to Elasticsearch for historical search.
- [alarm-config-logger](https://github.com/ControlSystemStudio/phoebus/tree/master/services/alarm-config-logger) - Phoebus service that tracks and logs Alarm Service configuration changes.
- [alh](https://github.com/epics-extensions/alh) - Alarm Handler: legacy GUI tool for monitoring and acknowledging EPICS alarms. Superseded by the Phoebus alarm system.

### Logging

- [phoebus-olog](https://github.com/Olog/phoebus-olog) - Online logbook service for experimental logging, integrated with the Phoebus ecosystem.
- [phoebus-olog-web-client](https://github.com/Olog/phoebus-olog-web-client) - ReactJS web client for the Phoebus Olog logbook service.
- [Olog Service](https://github.com/Olog/olog-service) - Java EE backend logbook service for EPICS experimental logging.
- [Olog logbook](https://github.com/Olog/logbook) - Lightweight HTML5/jQuery web client for Olog Service. Superseded by phoebus-olog-web-client.
- [ELOG](https://elog.psi.ch/elog/) - Lightweight electronic logbook widely used at physics facilities alongside EPICS (PSI).
- [py_elog](https://github.com/paulscherrerinstitute/py_elog) - Python client for reading and writing ELOG logbook entries (PSI).
- [ioclogserv2](https://github.com/mdavidsaver/ioclogserv2) - More flexible reimplementation of the EPICS IOC log server.

### IOC & Database Tools

- [VisualDCT](https://github.com/epics-extensions/VisualDCT) - Visual Database Configuration Tool: graphical editor for EPICS database files.
- [epicsdbbuilder](https://github.com/DiamondLightSource/epicsdbbuilder) - Python library for programmatically building EPICS database files (Diamond Light Source).
- [whatrecord](https://github.com/pcdshub/whatrecord) - IOC meta-information tool: parses EPICS databases, startup scripts, and snl programs.
- [dbtoolspy](https://github.com/paulscherrerinstitute/dbtoolspy) - Python module for reading and parsing EPICS database files (PSI).
- [ioc-clone](https://github.com/mdavidsaver/ioc-clone) - Captures a snapshot of PV values as a loadable `.db` file.
- [oac-tree](https://github.com/oac-tree/oac-tree-bundle) - Behavior-tree-based procedure sequencing framework for EPICS control systems.
- [phoebusgen](https://github.com/als-epics/phoebusgen) - Python library for generating Phoebus OPI display files programmatically.
- [phoebus-converter](https://github.com/ControlSystemStudio/phoebus-converter) - Converts legacy .opi (CSS/BOY) and .adl (MEDM) display files to Phoebus .bob format.
- [c2dataviewer](https://github.com/epics-extensions/c2dataviewer) - Python GUI front-end for visualizing AreaDetector and pvAccess image data.
- [GATO](https://github.com/epics-extensions/gato) - Legacy generator tool for EPICS display files. Archived.

### Simulators & Test IOCs

- [lewis](https://github.com/ISISComputingGroup/lewis) - Python framework for writing simulated hardware devices for testing EPICS IOC control systems.
- [epics-rs](https://github.com/epics-rs/epics-rs) - Pure-Rust EPICS Simulation framework: IOC core, CA, pvAccess, asyn, motor, areaDetector, and modbus ports.
- [EPICS-IOC-Demo](https://github.com/jeonghanlee/EPICS-IOC-Demo) - Simple example IOC (Asyn, Calc, StreamDevice) with a TCP/IP serial simulator.
- [ServiceTestIOC](https://github.com/jeonghanlee/ServiceTestIOC) - Minimal IOC for testing EPICS middleware services.
- [tc32sim](https://github.com/jeonghanlee/tc32sim) - EPICS IOC simulator for TC-32 thermocouple devices.
- [epics-modbus-example](https://github.com/mdavidsaver/epics-modbus-example) - Example IOC using the modbus driver against a simulated PLC.
- [vxi11sim](https://github.com/mdavidsaver/vxi11sim) - Simple simulated VXI-11 server for testing instrument communication.

### Diagnostics & Network Analysis

- [cashark](https://github.com/mdavidsaver/cashark) - Wireshark dissector plugin for decoding EPICS Channel Access and pvAccess network traffic.
- [EpicsSniffer](https://github.com/paulscherrerinstitute/EpicsSniffer) - GUI tool for analyzing EPICS Channel Access traffic in real time and from pcap files (PSI).
- [archstats](https://github.com/pcdshub/archstats) - EPICS IOC providing Archiver Appliance health and statistics records (SLAC/PCDS).
- [ci-core-dumper](https://github.com/mdavidsaver/ci-core-dumper) - Automates analysis of core dumps from crashes during CI builds and test runs.

## Tutorials & Training

- [EPICS Training](https://github.com/epics-training) - GitHub organization of official EPICS training courses and hands-on materials.
- [training-collection](https://github.com/epics-training/training-collection) - Parent repo bundling all modules for an EPICS training course.
- [training-vm](https://github.com/epics-training/training-vm) - Flexible, maintainable EPICS training VM built with VirtualBox and Ansible.
- [epics7-overview](https://github.com/epics-training/epics7-overview) - Overview of EPICS 7 with examples from QSRV2, PVXS, and P4P.
- [phoebus-training](https://github.com/epics-training/phoebus-training) - Training material and references for Phoebus.
- [stream-introduction](https://github.com/epics-training/stream-introduction) - Introductory training for StreamDevice.
- [opcua-support](https://github.com/epics-training/opcua-support) - Introduction and hands-on for the EPICS OPC UA device support.
- [areadetector-training](https://github.com/epics-training/areadetector-training) - Hands-on training for areaDetector.
- [epics-trainings](https://github.com/jeonghanlee/epics-trainings) - EPICS environment training materials and exercises.
- [RTEMS Tutorial](https://github.com/anjohnson/RTEMS-tutorial) - Eric Norum's "Getting Started with RTEMS" tutorial and build scripts, for EPICS IOCs on RTEMS.

## Other Lists

- [EPICS Extensions](https://epics.anl.gov/extensions/index.php) - The following list gives access to individual pages for most of the standard EPICS host tools and CA clients.
- [EPICS SoftSupport](https://epics-controls.org/resources-and-support/modules/soft-support/) - The following table contains an index of EPICS Soft Support modules available for use within IOCs.
- [EPICS Related Software](https://docs.epics-controls.org/en/latest/software/epics-related-software.html) - The official EPICS documentation catalog of related software, modules, and tools.
- [Tango Controls](https://tango-controls.org/) - Free open-source device-oriented control system framework used widely at European facilities; the main open-source alternative to EPICS.
