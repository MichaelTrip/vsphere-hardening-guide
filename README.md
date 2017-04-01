# vsphere-hardening-guide
vSphere Hardening Guide Compliance Scripts</br>
Based on VMware's Hardening Guide, version 5.5</p>

All VMware Hardening Guides are homed at http://www.vmware.com/security/hardening-guides.html</br>
These scripts are used in <b>SANS SEC579</b>: https://www.sans.org/course/virtualization-private-cloud-security</p>
Scripts:</br>
audit-esxi.ps1      Audit ESXi specific checks</br>
audit-vnetwork-ps1  Audit network specific checks</br>
audit-vms.ps1       Audit all VMs</br>
audit-vc.ps1        Audit vCenter</p>

For usage:
- Open VMware PowerCLI
- Run the script with the target ESXi or vCenter host as the single argument
- Targeting a vCenter host will cover all attached ESXi hosts and VMs

Requirements:
- PowerShell version 4 or better is recommended ($PSVersionTable.PSVersion)
- PowerCLI version 5.5 release 1 or newer (Get-PowerCLIVersion)
- NMAP is required for some audit tests - install the latest version of nmap from https://nmap.org/download.html

The vCenter audit script is optimized for Windows installs, but will still run fine against the Appliance version of VC

Enjoy!
