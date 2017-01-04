# ansible-role-cronacle
A role to download, install and upgrade [Redwood's](https://www.redwood.com) [Cronacle](https://www.cronacle.com) using [Ansible](https://www.ansible.com).

## Requirements

### Dependencies
- RedwoodSoftware/ansible-role-java
         
### Role Defaults (defaults)

The available defaults are listed below with a brief explanation of their meaning:

```yaml
version:       The version of Cronacle you want to install, or upgrade to, for instance: "9.0.20.0" 
               Please login to your account to determine which versions are available. 
          
cronacle:
  owner:       The user which owns the installation tree
  group:       The group set on the installation tree
  installDir:  The directory where to install Cronacle.
  packagePath: The directory to which the installation package is downloaded.
  packageName: The destination name of the package which is stored in packagePath.
  selfUpgrade: Whether Cronacle is allowed to automatically upgrade when a newer WAR file is detected.
  maxMem:      The Maximum Heap Size for the JVM (-Xmx)
  jmx:         Enables (unprotected) JMX on the JVM.
```       
       
### Role Variables (vars)

```yaml
redwoodPortal:
  username: Your Redwood Software Support Portal user account.
  password: The corresponding password for this account.
```

## Warranty
This role is provided as is and does not come with any form of support.

