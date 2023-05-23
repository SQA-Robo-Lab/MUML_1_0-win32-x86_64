# The MechatronicUML Tool Suite

The MechatronicUML Tool Suite (MUML TS) is an Eclipse-based IDE for using the [MechatronicUML](http://www.mechatronicuml.org/de/index.html). 

It can be installed through a VirtualBox image that can be found at the bottom of the [dowload section on the MUML homepage](http://www.mechatronicuml.org/en/download.html).

All other download options there are not working anymore, therefore we provide an alternative download here via this GitHub repository for a direct installation on Windows.

## Installation Instructions

1) Download the zip-File linked under "Releases", unzip it.
2) Install a Java 8 VM if you don't have one on your local machine.
3) If you work with multiple JVMs on your machine (or if you just want to be explicit): configure the Java 8 VM as runtime environment for the MUML TS by editing the eclipse.ini file in the unzipped directory. Add 
```
-vm
<path-to-your-java8vm>
```
4) Start the MUML TS by executing the eclipse.exe in the unzipped directory.

## Install the Plugins

To use the plugins for code generation, they have to be installed first.
The simplest way to do this is to clone the repositories of the plugins and import the contained Eclipse plugin projects into the workspace of the MUML TS.

Clone and import the following plugins and choose the correct branch (I recommend to use ```File > Import > Git > Projects from Git > CloneURI```):
* https://github.com/fraunhofer-iem/mechatronicuml-core (branch: master)
* https://github.com/fraunhofer-iem/mechatronicuml-pim (branch: master)
* https://github.com/fraunhofer-iem/mechatronicuml-pm (branch: master)
* https://github.com/fraunhofer-iem/mechatronicuml-psm/tree/stuerner_ma (branch: stuerner_ma)
* https://github.com/fraunhofer-iem/mechatronicuml-cadapter-component-container (branch: stuerner_ma)
* https://github.com/fraunhofer-iem/mechatronicuml-cadapter-component-type (branch: stuerner_ma)

Now right click on one of the imported projects and choose ```Run As > Eclipse Application```.
A new Eclipse window will appear that contains all features of the MUML TS with the plugins installed.

## Troubleshooting

It can happen that some imported plugins have errors that prevent the MUML Tool Suite from starting correctly or displaying certain diagram types.

In some cases, removing the affected plugin and re-importing it solves this issue.

If that doesn't work, go the the file of the plugin that contains the error.
Sometimes, the import of some classes can be missing, which causes the issue.
Add the import through a suggestion by Eclipse and the error should be resolved.
