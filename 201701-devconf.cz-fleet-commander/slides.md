<!-- $theme: gaia -->

Introduction to Fleet Commander
-------------------------------

DevConf.cz 2017
Oliver Gutierrez
![Alt text](fc-logo.png)

---

Large workstation deployments
=============================

A hell for the sysadmins

Main tasks:

* Deploy software on machines and configure them
* Deploy user configuration and personal files

---

Deploying machines
==================

* Configuration management systems
	* Ansible
	* Chef
	* Puppet
	* ...

---

Deploying profiles
==================

* APOC (2006)
* Sabayon (2007)
* ??? (usually custom made scripts)


---

Fleet Commander
===============

  * Easy to manage profiles
  * Easy to add settings to that profiles
  * Easy to deploy that profiles to the network
  * Transparent experience for the final user

---

Easy to manage profiles
=======================

* Graphic session for software configuration (SPICE, Libvirt, SSH)
* Web forms for specifying special configurations

---

Easy to deploy
==============

* Minimal software installation on client machines for applying configuration at login time
* Minimal configuration on client machines to retrieve profile data and apply it

---

Fleet Commander components
==========================

* Fleet Commander Admin
* Fleet Commander Logger
* Fleet Commander Client

---

Fleet Commander Admin
=====================

* Profile management
* Web based (Cockpit plugin)
* dbus service as backend

---

Fleet Commander Logger
======================

* Logs configuration changes during Live Sessions
* Transfer that changes to Fleet Commander Admin for reviewing
* Only needed in template virtual machines
* Only activates in Fleet Commander live sessions

---

Fleet Commander Client
======================

* Downloads profiles from profile server (This will change with FreeIPA integration)
* Compiles all profiles that applies to user at login time
* Applies the configuration

---

Supported settings
==================

* Web interface
  * Gnome Software highlighted applications
  * Gnome Online Accounts (In progress)

* Live Session
  * GSettings based Applications
  * LibreOffice
  * Network manager (preconfiguration of VPN, WiFi...)

---

Future releases
===============

* In progress integration with FreeIPA
* Enhancements in UI and UX

---

Demo
====

![Alt text](fc-logo.png)

---

Project information
-------------------
Source code at GitHub:
* <https://github.com/fleet-commander/>

GNOME Wiki documentation
* <http://wiki.gnome.org/Projects/FleetCommander>

Contact me
----------
ogutierrez (at) redhat (dot) com

---

THANK YOU
=========
