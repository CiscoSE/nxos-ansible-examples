# Demo Instructions
This script modifies a pair of NXOS 9K switches designated as "Edge" switches, and a pair of switches designated and "Core" switches.

<span style="color:red">* THIS IS NOT FOR PRODUCTION USE *</span>

## Modifications to the INI file
An inventory file is required to run this script, and an example file is provided. You must modify the user name and password for your switches, and set the IP address for each switch in the demoList of the sample INI file before running this script against a demo environment.

Once the INI file is modified, run the script using this methodology:

```
    ansible-playbook -i nameOfModifiedINIFile configDemo.yaml
```

