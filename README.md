# push_internal script

## What does it do?
This script can be used to trigger Jenkins jobs in the Cloud to push code to our internal network on-demand.

## How do I use it?
The script is quite simple: `push_internal [--all] [args..]`
 - `--all` pushes all projects in CAPI and CHP that have been pre-defined to be 'CHP Projects' that our team owns.
 - `args..` is a list of project names. These do not have to be CAPI or CHP Projects.
 	- If an argument is not specific enough and returns more than one job, the user will be prompted to choose which job they were referring to.
 - The flags can be used together or separate.

## System Requirements
- Python3
- python package Python-Jenkins
	- Can be installed by running `sudo pip install python-jenkins`
