# Awesome [EPICS](https://epics-controls.org/)

The Experimental Physics and Industrial Control System (EPICS) is a set of software tools and applications used to develop and implement distributed control systems to operate devices such as particle accelerators, telescopes and other large experiments.

* [Awesome EPICS](#awesome-epics)
  * [Base](#base)
    * [User Sites](#user-sites)
    * [Editor Extensions](#editor-extensions)
  * [Modules](#modules)
  * [Packaging](#packaging)
  * [IOC Runners](#ioc-runners)
  * [Applications](#applications)
  * [Other lists](#other-lists)

## Main EPICS Links

* [EPICS Tech Talk Mailing List](https://epics.anl.gov/tech-talk/) - The main forum for talking about EPICS and the other parts of the ecosystem.
* [EPICS Controls](https://epics-controls.org/) - The newer home for EPICS.
* [EPICS Argonne Home](https://epics.anl.gov/) - The older website hosted at Argonne National Laboratory.
* [EPICS Documentation](https://docs.epics-controls.org/en/latest/index.html)
* [EPICS Github Organization](https://github.com/epics-base)

## Base

* [EPICS Base](https://github.com/epics-base/epics-base) - EPICS is a set of Open Source software tools, libraries and applications developed collaboratively and used worldwide to create distributed soft real-time control systems for scientific instruments such as a particle accelerators, telescopes and other large scientific experiments.
* [EPICS Docs](https://github.com/epics-docs/epics-docs) - Documentation for EPICS Base.

### User Sites

* [ESS](https://europeanspallationsource.se/) - The European Spallation Source (ESS) is a European Research Infrastructure Consortium (ERIC), a multi-disciplinary research facility based on the world’s most powerful neutron source.
* [PSI](https://www.psi.ch/en) - The Paul Scherrer Institute PSI is the largest research institute for natural and engineering sciences in Switzerland, conducting cutting-edge research in four main fields: future technologies, energy and climate, health innovation and fundamentals of nature.
* [ANL](https://www.anl.gov/) - Argonne is a multidisciplinary science and engineering research center, where talented scientists and engineers work together to answer the biggest questions facing humanity, from how to obtain affordable clean energy to protecting ourselves and our environment. 
* [Diamond Light Source](https://www.diamond.ac.uk/) - Diamond Light Source is the UK’s national synchrotron. It works like a giant microscope, harnessing the power of electrons to produce bright light that scientists can use to study anything from fossils to jet engines to viruses and vaccines.

### Editor Extensions

* [vscode](https://github.com/epics-extensions/vscode-epics) - VS Code colorization for EPICS database, templates and substitution files.

### Network Protocols

#### pvAccess

pvAccess is a high-performance network communication protocol for signal monitoring and scientific data services interconnect.

* [pvAccess Specifiction](https://github.com/epics-base/pvAccessCPP/wiki/Protocol-Encoding)
* [Original C++ Implementation](https://github.com/epics-base/pvAccessCPP)
* [pvxs C++ Implementation](https://mdavidsaver.github.io/pvxs/index.html)
* [Original Java Implementation](https://github.com/epics-base/epicsCoreJava/tree/3a32ca5dbc2fd9db610c3d7c08e37600b9aa0b32/pvAccessJava#readme)
* [Phoebus Java Implementation](https://github.com/ControlSystemStudio/phoebus/tree/master/core/pva)

#### Channel Access

* [Channel Access Specification](https://docs.epics-controls.org/en/latest/specs/ca_protocol.html)
* [Java Implementation](https://github.com/epics-base/jca)
* [pyepics](https://github.com/pyepics/pyepics) - PyEpics is a Python interface to the EPICS Channel Access (CA) library for the EPICS control system.

## Modules

* [asyn](https://github.com/epics-modules/asyn) - EPICS module for driver and device support.
* [StreamDevice](https://github.com/paulscherrerinstitute/StreamDevice) - EPICS Driver for message based I/O.
* [recsync](https://github.com/ChannelFinder/recsync) - EPICS Record Synchronizor.
* [mca](https://github.com/epics-modules/mca) - EPICS support for multi-channel analyzers (MCA) and multi-channel scalers (MCS).

## Packaging

* [e3](https://gitlab.esss.lu.se/e3/e3) - Allows for easily building EPICS modules directly from source and automagically resolves module dependencies, and allows for site-specific modifications to EPICS modules without needing to directly modify source trees.
* [EPNix](https://epics-extensions.github.io/EPNix/nixos-25.11/) - EPNix (pronunciation: as if you are high on mushrooms) enables you to build, package, deploy IOCs and other EPICS-related software by using the Nix package manager.
* [EPICS Containers](https://github.com/epics-containers) - A collection of tools and documentation for building, deploying and managing containerized EPICS IOCs in a Kubernetes cluster.

## IOC Runners

## Applications

* [Channel Finder](https://github.com/ChannelFinder/ChannelFinderService) - A RESTful directory services for a list channels.
* [Archiver](https://github.com/archiver-appliance/epicsarchiverap) - This is an implementation of an archiver for EPICS control systems that aims to archive millions of PVs.
* Alarm Service
* [Phoebus](https://github.com/ControlSystemStudio/phoebus) - A framework and set of tools to monitor and operate large scale control systems, such as the ones in the accelerator community.
* [CS Studio](https://github.com/ControlSystemStudio/cs-studio) - Control System Studio is an Eclipse-based collections of tools to monitor and operate large scale control systems, such as the ones in the accelerator community.

## Other Lists

* [EPICS Extensions](https://epics.anl.gov/extensions/index.php) - The following list gives access to individual pages for most of the standard EPICS host tools and CA clients.
* [EPICS SoftSupport](https://epics-controls.org/resources-and-support/modules/soft-support/) - The following table contains an index of EPICS Soft Support modules available for use within IOCs.

