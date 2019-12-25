# SwitchHost
Switch IP adresses easily in hosts file.
Useful when your VM changes IP address when you change location for instance.

## Requirements
None, it's just a plain shell script to execute.

## Usage
- Edit the list of "locations" and "IP addresses" in the `switchhost.sh` file
- Make a copy of `hosts-template-example` and rename it `hosts-template`
- List the hosts you want to be dynamic in the `hosts-template` file
- Keep `hosts-template` and `switchhost.sh` in the same folder
- Change the value of the variable `hostpath` in `switchhost.sh` if your hosts file is not located in `/etc`
- Set permissions on the script : `chmod u+x switchhost.sh`
- Execute the script and select the location :

    ```bash
    sudo ./switchhost
    ```

## TODO
- Add checks if files exist, etc. (https://linuxize.com/post/bash-check-if-file-exists/)