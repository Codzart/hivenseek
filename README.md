# hivenseek
Quick and Dirty tool to scan for evidence of CIA's "hived" agent on Linux devices.

From the WikiLeaks 'Vault 7' disclosure, a system designated 'hive' is described.
https://wikileaks.com/ciav7p1/

Within the HIVE Developers Guide, a self-delete mechanism is documented to leave behind tell-tale signs of an active or abandoned implant of the hived agent.
https://wikileaks.com/ciav7p1/cms/files/DevelopersGuide.pdf

This lightweight tool, 'hivenseek' was constructed to look for these signs on \*nix-like systems and report any such evidence.


# OVERVIEW
hivenseek is a bash script(compiled with shc Version 3.8.7) that performs passive read-only operations. It is intended to run without modification on a variety of Linux-based systems.   The underlying bash code is shrouded in the executable, but is discoverable on a running system in the process title if you care to review it.  It may be released here in coming months for adaptation to other systems.
The expiry date is currently 2018MAR15.  By then, I hope this will no longer be of any interest to anyone.

# INSTALLATION and USAGE
Download the executable
```bash
wget https://github.com/Codzart/hivenseek/raw/master/hivenseek
chmod 550 hivenseek
```

Verify the executable
```bash
sha256sum hivenseek 
28b83a9a147aeab25b5dd1d7eeacc9fce77c07693e4679ec7287e505f38c8b83  hivenseek (v2017.3.11)
86661c0104c1d0e96a05e4ccc86760aa4b7968ef172661778b1578ff4ff9e36c  hivenseek (v2017.3.12)
```
Run the executable
```bash
# hivenseek Usage: hivenseek [-auto] 

./hivenseek 
```

Without arguments, an explanatory prompt is printed, requesting permission to proceed.

With the *-auto* option, no prompt is given and the scan begins immediately.




hivenseek can be called from most common automation systems.

No SIEM or syslogging formats are planned for the first version.

# REPORTING
hivenseek provides the option to anonymously report the result of the scan (active/abandoned/absent,time,address)

# DONATIONS
This small tool is happily placed in the public domain, but the author welcomes donations.

bitcoin:13cAKxc4CHjSYsovxSP5k2RzBmUtzvjLbC?amount=0.1&label=hivenseek&message=donation

```
█████████████████████████████████████████
██ ▄▄▄▄▄ █▀█ █▄ ▀ █  ▄  ▄▄▄▀█ ▄█ ▄▄▄▄▄ ██
██ █   █ █▀▀▀█ ▄▀█▄▀▀█▄▄█▀█▀▀█▀█ █   █ ██
██ █▄▄▄█ █▀ █▀▀██▀ ▀▄▄ █▀▄ ▄▀▀▄█ █▄▄▄█ ██
██▄▄▄▄▄▄▄█▄▀ ▀▄█ █ █ █ ▀▄█▄█ █▄█▄▄▄▄▄▄▄██
██▄▄ ▄ █▄▄▄ ▀▄▀▀▀█▀ ▀▀▀▀▀▀██   ▄█ █ ▀▄███
██ ▄▀▄▄▄▄ █▀██▀ ▄ ▄██▀▄ ▀▀▄█ ▄████▀██ ▄██
██ █ ▄  ▄█▄ ▄█▄█▄█▀▄▀▀ ▀█ ▄▄ ▄▄  ▀█▄ ▄███
███▄▄▀██▄▄▄█  ▄█▀ ▀██▀▀▀▄███▄▄▄▀▄▄▄ ▄ ▄██
██▀▄▄▄  ▄ ▄ █▄▀▀▀▄ ▄█ ▀█▄▀█  █▀  ▀█▀ █▄██
██▀ █  █▄▄▄ ▄█▀ ▄ ▄▄▄█  ▄▀█▄█  ▀▀▀█ ▄▄ ██
██▄█▄█▀█▄  ▄ █▄█▄▄▀▄█▀▀▀▄ ▄▄ ▄▄ ▄▄▄▀▄ ▄██
███▀▄ ██▄ ▄██ ▄█▀▄▀▄▄▀▀ ▀██▄▄ █▀▄▄▄▀█  ██
██ ▄██▄▀▄▀ ▄▄▄▀▀▀█▀▄▀▀ ▀▄ ▄ ▄  ▄▄▀▄▀▄████
██ █ ▀▄▀▄  ▄▄█▀ ▄▄ █▄█▄▀██▀▄█▄▄ ██▀█▄▄▄██
██▄██▄██▄▄  ▄█▄█▄█▀▄▀ ▀▀▄▀▄▀▄▄ ▄▄▄  ▄█▄██
██ ▄▄▄▄▄ █▄▄▀ ▄█▀ ▀▄███  ▀██▄▄ █▄█ █▄▄▄██
██ █   █ █  █▄▀▀▀▄▀▄▀ ▀█▄ ▀▄▄ ▄     █  ██
██ █▄▄▄█ █ █▄█▀ ▄  ███  ▄▀▀▄█▄  ▀ ▀██▄ ██
██▄▄▄▄▄▄▄█▄▄▄█▄█▄█▄▄▄▄▄███▄█▄█████▄▄█▄▄██
█████████████████████████████████████████
```

