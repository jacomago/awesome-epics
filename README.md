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

### Network Protocols

#### pvAccess

pvAccess is a high-performance network communication protocol for signal monitoring and scientific data services interconnect.

* [pvAccess Specification](https://github.com/epics-base/pvAccessCPP/wiki/Protocol-Encoding)
* [Original C++ Implementation](https://github.com/epics-base/pvAccessCPP) _(archived)_
* [pvxs C++ Implementation](https://mdavidsaver.github.io/pvxs/index.html)
* [Original Java Implementation](https://github.com/epics-base/epicsCoreJava/tree/3a32ca5dbc2fd9db610c3d7c08e37600b9aa0b32/pvAccessJava#readme) _(archived)_
* [Phoebus Java Implementation](https://github.com/ControlSystemStudio/phoebus/tree/master/core/pva)

#### Channel Access

* [Channel Access Specification](https://docs.epics-controls.org/en/latest/specs/ca_protocol.html)
* [Java Implementation](https://github.com/epics-base/jca)
* [pyepics](https://github.com/pyepics/pyepics) - PyEpics is a Python interface to the EPICS Channel Access (CA) library for the EPICS control system.

## Modules

* [asyn](https://github.com/epics-modules/asyn) - EPICS module for driver and device support.
* [StreamDevice](https://github.com/paulscherrerinstitute/StreamDevice) - EPICS Driver for message based I/O. _(site-PSI)_
* [recsync](https://github.com/ChannelFinder/recsync) - EPICS Record Synchronizor.
* [mca](https://github.com/epics-modules/mca) - EPICS support for multi-channel analyzers (MCA) and multi-channel scalers (MCS).

## Packaging

* [e3](https://gitlab.esss.lu.se/e3/e3) - Allows for easily building EPICS modules directly from source and automagically resolves module dependencies, and allows for site-specific modifications to EPICS modules without needing to directly modify source trees. _(site-ESS)_
* [EPNix](https://epics-extensions.github.io/EPNix/nixos-25.11/) - EPNix (pronunciation: as if you are high on mushrooms) enables you to build, package, deploy IOCs and other EPICS-related software by using the Nix package manager.
* [EPICS Containers](https://github.com/epics-containers) - A collection of tools and documentation for building, deploying and managing containerized EPICS IOCs in a Kubernetes cluster.

## IOC Runners

* [procServ](https://github.com/ralphlange/procServ) - Process server: wraps an IOC (or any child process) with a telnet console and automatic restart.

## Applications

* [Channel Finder](https://github.com/ChannelFinder/ChannelFinderService) - A RESTful directory service for a list of channels.
* [Archiver](https://github.com/archiver-appliance/epicsarchiverap) - This is an implementation of an archiver for EPICS control systems that aims to archive millions of PVs.
* [Alarm Service](https://github.com/ControlSystemStudio/phoebus/tree/master/app/alarm) - EPICS alarm handling system, part of the Phoebus suite.
* [Phoebus](https://github.com/ControlSystemStudio/phoebus) - A framework and set of tools to monitor and operate large scale control systems, such as the ones in the accelerator community.
* [CS Studio](https://github.com/ControlSystemStudio/cs-studio) - Eclipse-based predecessor to Phoebus for monitoring and operating large scale control systems. Superseded by Phoebus. _(archived)_

## Other Lists

* [EPICS Extensions](https://epics.anl.gov/extensions/index.php) - The following list gives access to individual pages for most of the standard EPICS host tools and CA clients.
* [EPICS SoftSupport](https://epics-controls.org/resources-and-support/modules/soft-support/) - The following table contains an index of EPICS Soft Support modules available for use within IOCs.
