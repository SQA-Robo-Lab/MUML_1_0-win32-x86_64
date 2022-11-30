# The MechatronicUML Tool Suite

The MechatronicUML Tool Suite (MUML TS) is an Eclipse-based IDE for using the [MechatronicUML](http://www.mechatronicuml.org/de/index.html). As no working download is currently available on the web, we provide a download here via this GitHub repository.

## Installation instructions

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
