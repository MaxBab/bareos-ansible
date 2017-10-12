Bareos Ansible
--------------

### Bareos - Backup Archiving REcovery Open Sourced
Bareos (Backup Archiving Recovery Open Sourced) is a reliable, cross-network
open source software for backup, archiving and recovery of data for all
well-established operating systems. Emerged from the Bacula Project in 2010,
Bareos was and is actively developed as a fork and enriched with lots of new features.

The following repo contains number of Bareos roles.
- Bareos basic - Sets Bareos repositories and holds common variables.
- Bareos database - Installs one of the following databases: Postgresql/MariaDB.
- Bareos Director - Installs and configures Bareos Director.
- Bareos WebUI - Installs and configures Bareos WebUI.
- Bareos clients - Installs and configures Bareos clients.

The bareos-basic role contains common variables that used by other roles (ex. passwords).  
Bareos-basic role triggered by the meta dependency of each role.

Please, use the inventory.example file as a reference for the required groups.

>Supported platforms:
- Centos 6
- Centos 7
- Debian 8
- Ubuntu 14.04

#### TODO:
- [x] Install and configure Bareos (Director, WebUI, Clients)
- [ ] SSL support
- [ ] Jobs creation
