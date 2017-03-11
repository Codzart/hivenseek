# hivenseek
Quick and Dirty tool to scan for evidence of CIA's "hived" agent on Linux devices.

From the WikiLeaks 'Vault 7' disclosure, a system designated 'hive' is described.
https://wikileaks.com/ciav7p1/

Within the HIVE Developers Guide, a self-delete mechanism is documented to leave behind tell-tale signs of an active or abandoned implant of the hived agent.
https://wikileaks.com/ciav7p1/cms/files/DevelopersGuide.pdf

This lightweight tool, 'hivenseek' was constructed to look for these signs on \*nix-like systems and report any such evidence.


# OVERVIEW
hivenseek is a bash script(compiled with shc Version 3.8.7) that performs passive read-only operations. It is intended to run without modification on a variety of Linux-based systems.   The underlying bash code is embedded in the executable, but discoverable on a running system.  It may be released here in coming months for adaptation to other systems.

# INSTALLATION and USAGE
Download the executable
```bash
wget https://github.com/Codzart/hivenseek/raw/master/hivenseek
chmod 550 hivenseek
hivenseek Usage: hivenseek [-auto] 

./hivenseek 
```

Without arguments, an explanatory prompt is printed, requesting permission to proceed.

With the *-auto* option, no prompt is given and the scan begins immediately.




hivenseek can be called from most common automation systems.

No SIEM or syslogging formats are planned for the first version.

