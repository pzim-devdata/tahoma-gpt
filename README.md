# tahoma-gpt
[UP TO DATE] Tahoma-gpt is an addon for [tahoma by pzim-devdata](https://github.com/pzim-devdata/tahoma/tree/main) for controlling Somfy Tahoma devices using ChatGPT and for getting help about tahoma by pzim-devdata



<p align="center" width="100%">
    <img width="15%" src="https://github.com/pzim-devdata/tahoma/blob/main/tahoma-gpt.png"> 
</p>



[![GitHub license](https://img.shields.io/github/license/pzim-devdata/tahoma?style=plastic)](https://github.com/pzim-devdata/tahoma-gpt/blob/main/LICENSE)    ![](https://img.shields.io/badge/Works%20with-Python%203-red?style=plastic)    ![GitHub issues](https://img.shields.io/github/issues/pzim-devdata/tahoma-gpt?style=plastic)    [](https://github.com/pzim-devdata/tahoma-gpt/issues)    ![GitHub repo size](https://img.shields.io/github/repo-size/pzim-devdata/tahoma-gpt?style=plastic)    [![Visits Badge](https://badges.strrl.dev/visits/pzim-devdata/tahoma-gpt)](https://badges.strrl.dev)    ![GitHub release (latest by date)](https://img.shields.io/github/v/release/pzim-devdata/tahoma-gpt?style=plastic)    [![GitHub commits](https://img.shields.io/github/commits-since/pzim-devdata/tahoma-gpt/v2.2.0.svg?style=plastic)](https://GitHub.com/pzim-devata/tahoma-gpt/commit/)    
<!---
THIS TAG DOESN'T WORK, DON'T TRUST IT : ![GitHub All Releases](https://img.shields.io/github/downloads/pzim-devdata/tahoma-gpt/total?style=plastic) 
-->
[![Downloads](https://static.pepy.tech/personalized-badge/tahoma?period=total&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads)](https://pepy.tech/project/tahoma-gpt) 

[Pypi project](https://pypi.org/project/tahoma-gpt/)
# Features

![Picture tahoma-gpt](https://github.com/pzim-devdata/tahoma/blob/main/picture_tahoma-gpt.png)


- Control Somfy Tahoma devices with a simple API written in Python 3
- Create scripts or shortcuts to controle your house from a domestic server or your computer
- With this API, you can integrate Somfy's products with other Matter-compatible devices
- Works with Somfy Connectivity Kit, Connexoon, Cozytouch, and more
- Support various Somfy's devices: alarm, shutter, plug, heater, sensors, scenes, and more
- Compatible with Windows and Linux operating systems
- 100% functional with ChatGPT


# Easy Process to Test and Install tahoma and tahoma-gpt

If you want to install Tahoma and Tahoma-GPT using a simple script on Linux, follow these steps:

1. Open your terminal (for Linux) or Powershell as asministrator (for Windows) and navigate to the directory where you want to download the script `install_tahoma-gpt.sh` for Linux and `install_tahoma_gpt_windows.bat` for Windows.

   For example for Linux:
   - `mkdir $HOME/tahoma-gpt`
   - `cd $HOME/tahoma-gpt`

   For exemple for Windows:
   - `New-Item -ItemType Directory -Path "C:\tahoma-gpt"`
   - `Set-Location -Path "C:\tahoma-gpt"`
   - `Set-ExecutionPolicy RemoteSigned`
 
3. Download the script `install_tahoma-gpt.sh` using the following command:

For Linux :

   - `wget -O "install_tahoma-gpt.sh" "https://github.com/pzim-devdata/tahoma/raw/main/install_tahoma-gpt.sh"`

   For Windows :

   - `Invoke-WebRequest -Uri "https://github.com/pzim-devdata/tahoma/raw/main/install_tahoma_gpt_windows.bat" -OutFile "install_tahoma_gpt_windows.bat"`


5. Make the installation script executable (Linux only) by running the following command:

   - `chmod +x install_tahoma-gpt.sh`
    
6. Execute the installation script in the terminal using the following command:

For Linux :

   - `bash -c './install_tahoma-gpt.sh'`

For Windows :

   - `& "./install_tahoma_gpt_windows.bat"`

7. You can now execute tahoma_chatgpt.sh for Linux or tahoma_chatgpt.bat for Windows or run tahoma-gpt.py in a vitual env (exemple for Linux):

   - `cd $HOME/tahoma-gpt` or ` cd c:\tahoma-gpt` (for Windows) (or go to the installed folder with the terminal)
   - `python3 -m venv env` or ` python -m venv env` (for Windows)
   - `source env/bin/activate` or `.\env\Scripts\activate` (for Windows)
   - `python3 tahoma-gpt.py` or `python tahoma-gpt.py` (for Windows)
   
     If you want to run tahoma without tahoma-gpt in the same virtual environnement:
     
   - `python3 tahoma.py` or `python tahoma.py` (for Windows) and follow instructions [there](https://github.com/pzim-devdata/tahoma#4-retrieve-your-personal-commands)

8. You can also execute orders as arguments :
     
   - For Linux :

      `bash -c 'tahoma_chatgpt.sh could you please open the shutter in the kitchen ?'`

     or
     
   - For Windows :

     `.\tahoma_chatgpt.bat could you please open the shutter in the kitchen ?`


By following these steps, Tahoma and Tahoma-GPT will be installed on your Linux or Windows system in a virtual environnement. 
You can execute  `bash -c 'tahoma_chatgpt.sh'` for Linux or `.\tahoma_chatgpt.bat` for Windows to run it in the folder of tahoma-gpt.


# Step by steps process to Test and Install tahoma and tahoma-pgt

- ### To install tahoma and tahoma-gpt in a virtual environnement :

You can create a vitual environnement in Python if you want to test it first. All will be installed in the tahoma-gpt directory

First you must install venv : `pip install virtualenv` or `python3 -m pip install virtualenv` or `pipx install virtualenv` to install vitual environnement
1. Create a directory with `tahoma-gpt.py` and `requirements_tahoma-gpt.txt` inside. Download from [there](https://github.com/pzim-devdata/tahoma/blob/main/requirements_tahoma-gpt.txt) and [there](https://github.com/pzim-devdata/tahoma/blob/main/tahoma-gpt.py)
2. Open a terminal
3. `cd` in the directory you have just created
4. Run : `python3 -m venv env` (Windows : ` python -m venv env`)
5. Run : `source env/bin/activate` (Windows : `.\env\Scripts\activate`)
6. Install tahoma and configure it (if it's not already done) :

    6.1. Run : `python3 -m pip install -U tahoma` or `python -m pip install -U tahoma`

    6.2 Configure tahoma : `tahoma -c`

    6.3 Get the list of your devices : `tahoma -g`

7. Run : `python3 -m pip install -r requirements_tahoma-gpt.txt` or `python -m pip install -r requirements_tahoma-gpt.txt`
8. Modify the script `tahoma-gpt.py` with a notepad to add OpenAI API key
9. Run : `python3 tahoma-gpt.py` or `python tahoma-gpt.py`
10. Play with tahoma and ChatGPT
11. Run : `exit` (to leave tahoma-gpt)
12. Run : `exit()` (to leave Python)
13. Run : `deactivate` (to deactivate the vitual environnement)

- ### To reload tahoma-gpt after this installation in a virtual env :

1. Run : `python3 -m venv env` (Windows : ` python -m venv env`)
2. Run : `source env/bin/activate` (Windows : `.\env\Scripts\activate`)
3. Run tahoma-gpt with tahoma : `python3 tahoma-gpt.py` (Windows :`python tahoma-gpt.py`)
4. If you only wants to run tahoma without tahoma-gpt : `python3 tahoma.py` (Windows :`python tahoma.py`)
5. Run : `deactivate` (to deactivate the vitual environnement)

- ### To uninstall tahoma and tahoma-gpt just remove the installation folder (tahoma-gpt)

You can find explanation about tahoma.py  from the original git of tahoma [there](https://github.com/pzim-devdata/tahoma#4-retrieve-your-personal-commands)
-------------------------------------------------------------------------------------

For :


Somfy Connectivity Kit
Somfy Connexoon IO
Somfy Connexoon RTS
Somfy TaHoma
Somfy TaHoma Beecon
Somfy TaHoma Switch
Thermor Cozytouch
And more...

Supported devices :
Alarm
Shutter
Plug
Heater
Sensors
Scenes
and more if you ask me on github : 

[@pzim-devdata GitHub Pages](https://github.com/pzim-devdata/tahoma/issues)












<p align="center" width="100%">
    <img width="33%" src="https://avatars.githubusercontent.com/u/52496172?v=4"> 
</p>

------------------------------------------------------------------

- [Licence](https://github.com/pzim-devdata/DATA-developer/raw/master/LICENSE)
MIT License Copyright (c) 2023 pzim-devdata

------------------------------------------------------------------

Created by @pzim-devdata - feel free to contact me!
