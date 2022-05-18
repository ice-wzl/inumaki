## Inumaki! 🦴
<img src='https://img.shields.io/badge/NeoVim-%2357A143.svg?&style=for-the-badge&logo=neovim&logoColor=white'/> <img src ='https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue'/> <img src='https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white'/> 

- [⚠️ **disclaimer**](https://github.com/cr-0w/inumaki#-disclaimer)
- [💽 **download**](https://github.com/cr-0w/inumaki#-installation)
- [📜 **to-do**](https://github.com/cr-0w/inumaki#to-do-)
- [💖 **credits**](https://github.com/cr-0w/inumaki#credits-)

`inumaki!` is a command-line tool written in python which helps remove the tedium of common capture-the-flag 'shell searching'. It's also `my first official project!` We've all been there; a bit of time has passed since our enumeration and we're finally ready to run a reverse shell on our target. However, soon, you're 30 tabs deep in some random blog posts trying to find out the syntax for *that one command* you know you should've memorized by now but couldn't be bothered to. You give up, head over to pentestmonkey, or read through your old notes in an attempt to find that elusive command, and finally, after the motherboard on your target has corroded because of how long it's been, you finally find it; swearing thereafter to remember that command so you never forget it again.

https://user-images.githubusercontent.com/59679082/168722637-88da267c-6d73-414f-8f56-8dc8c56ba6b8.mp4

> Okay, yes. That's *quite* the exaggeration, but it's really annoying! Anyways, inumaki will make it so that you can just type in the language you need a shell for, and it will spit out the most common ones used in CTFs!

## ⚡ Disclaimer! 
This tool generates reverse shell commands. However, keep in mind that obfuscation does not exist yet. **OPSEC wise, this tool is the equivalent of running head first into a wall made completely out of megaphones announcing your every move. Speaking of reverse shells**...

- DO NOT use these shells, or *any* commands such as these on hosts which you do not have EXPLICIT WRITTEN permission to do so.
- The author of `inumaki!` will not be held responsible if you decide to use this against someone or something you don't have permission to attack. Be smart, guys.
- This tool is going to be an evergrowing project, please report any bugs, issues, etc. and I'll try my absolute best to get the issues resolved. This *is* my first official project so I *am* still learning, but hopefully I can keep up.

## ⭐ Installation
```
git clone https://github.com/cr-0w/inumaki.git && cd inumaki
python3 -m pip install -r requirements.txt
chmod +x inumaki
```
## 🩸 Usage 
There are many ways to run the `inumaki` script. Ff you followed the instructions above, it should be stored in `/usr/local/bin` or some other entry in your `$PATH` so that you can call the script from anywhere. 
```
cr0w@blackbird:~$ inumaki
```
The script also works with `user-supplied arguments`. If you'd like to skip the whole one-by-one entries for the various parameters the script uses, you can pass them into the command line as follows:
```
inumaki -i 10.0.0.1 -p 9999 -s <shell>
inumaki -i $ip -p $port -s <shell>
```
As stated before, this script is ever growing, so, more shells are surely on their way once I get the time to incorporate them in. To list the *currently compatible* shells, run the script with `--list-shells`:
```
inumaki --list-shells

[+] the accepted shells are  'POWERSHELL', 'PYTHON3', 'PYTHON', 'BASH', 'PERL', 'RUBY', 'LUA', 'PHP', 'SH', 'NC'
```

## To-Do 📑
- <del>`create support for user-supplied arguments`</del> ✅ 
- `add more shells/languages`
- `add an auto listener initializer for shells like nc, python, etc.`

```
[for the future]
```

- `obfuscated shells?` <br>
- `support for windows?`
- `what else? hmm...`

## Credits 💖
A special thank you goes out to **swisskyrepo (swissky)** and the awesome `PayloadsAllTheThings` repository!
> Honestly, you might just be better off using that repo instead of my tool 😂 However, most, if not, all of the shells are directly from the following:</br>
@[swisskyrepo](https://github.com/swisskyrepo),
[PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/Reverse%20Shell%20Cheatsheet.md)
