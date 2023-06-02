`🦴 inumaki!`
---
<img src='https://img.shields.io/badge/NeoVim-%2357A143.svg?&style=for-the-badge&logo=neovim&logoColor=white'/> <img src ='https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue'/> <img src='https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white'/> 

- [⚠️ **disclaimer**](https://github.com/cr-0w/inumaki#-disclaimer)
- [💽 **download**](https://github.com/cr-0w/inumaki#-installation)
- [🎉 **usage**](https://github.com/cr-0w/inumaki#-usage)
- [📜 **to-do**](https://github.com/cr-0w/inumaki#-to-do)
- [💖 **credits**](https://github.com/cr-0w/inumaki#-credits)

`inumaki!` is a command-line tool written in python which helps remove the tedium of common capture-the-flag reverse shell payload searching.

https://user-images.githubusercontent.com/59679082/168722637-88da267c-6d73-414f-8f56-8dc8c56ba6b8.mp4

## ⚡ Disclaimer! 
This tool generates reverse shell commands. However, keep in mind that obfuscation for some of the shells does not exist yet.

- DO NOT use these shells, or *any* commands such as these on hosts which you do not have EXPLICIT WRITTEN permission to do so.
- The author of `inumaki!` will not be held responsible if you decide to use this against someone or something you don't have permission to attack. Be smart, guys.
- This tool is going to be an evergrowing project, please report any bugs, issues, etc. and I'll try my absolute best to get the issues resolved. This *is* my first official project so I *am* still learning, but hopefully I can keep up.

## ⭐ Installation
```
git clone https://github.com/cr-0w/inumaki.git && cd inumaki/
python3 -m pip install -r requirements.txt
chmod +x inumaki.py
```

## 🩸 Usage 
```
cr0w@blackbird:~$ inumaki -h
usage: inumaki [-h] [-i ip] [-p port] [-s shell] [-l] [-v]

generate common shells used during CTFs!

options:
  -h, --help            show this help message and exit
  -i ip, --ip ip        LHOST
  -p port, --port port  LPORT
  -s shell, --shell shell
                        SHELL
  -l, --list-shells     outputs the currently compatible shells (more shells are planned to be included in the future :))
  -v, --version         prints version
```
The script also works with `user-supplied arguments (from v1.1 onwards)`. If you'd like to skip the whole one-by-one entries for the various parameters the script uses, you can pass them into the command line as follows:
```
inumaki -i 10.0.0.1 -p 9999 -s <shell>
inumaki -i $ip -p $port -s <shell>
```
As stated before, this script is ever growing, so, more shells are surely on their way once I get the time to incorporate them in. To list the *currently compatible* shells, run the script with `-l or --list-shells`:
```
inumaki --list-shells

[+] the accepted shells are  'POWERSHELL', 'PYTHON3', 'PYTHON', 'BASH', 'PERL', 'RUBY', 'LUA', 'PHP', 'SH', 'NC'
```

## 📑 To-Do 
- <del>`create support for user-supplied arguments`</del> ✅ 
- `add more shells/languages`
- `add in some download cradles/QoL stuff?`
- `add an auto listener initializer for shells like nc, python, etc.`

```
[for the future]
```

- `obfuscated shells?` <br>
- `support for windows?`
- `...`

## 💖 Credits 
A special thank you goes out to **swisskyrepo (swissky)** and the awesome `PayloadsAllTheThings` repository!
> Honestly, you might just be better off using that repo instead of my tool 😂 However, most, if not, all of the shells are directly from the following:</br>
@[swisskyrepo](https://github.com/swisskyrepo),
[PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Reverse%20Shell%20Cheatsheet.md)
