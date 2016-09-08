# Droid Module: droid/sshd-config

Modify `/etc/ssh/sshd_config`. For more information on Droid, please see
[droidphp.com](http://droidphp.com).

The steps involved are:-

1. Write a list of Option Argument tuples to `/etc/ssh/sshd_config`.
2. Restart the SSH service if the config file is changed as a result of the
   previous step.


## Assumptions

1. The platform is Debian-based.
2. The SSH Service is already installed.


## Limitations

None.


## Information required by the module

1. One or more Inventory Hosts, having a `public_ip`.
2. A list of Option Argument tuples (yaml arrays):-

        sshd_config:
          - [ <string>, <string> ] # for example, [PasswordAuthentication, no]
          - ...

## Optional information

None.
