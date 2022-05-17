## inumaki! 🦴
<center><img src='https://img.shields.io/badge/NeoVim-%2357A143.svg?&style=for-the-badge&logo=neovim&logoColor=white'/> <img src ='https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue'/> <img src='https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kali-linux&logoColor=white'/> 

**inumaki!** is a command-line tool written in python which helps remove the tedium of common capture-the-flag 'shell searching'. it's also my first official project! we've all been there; a bit of time has passed after our enumeration and we're finally ready to run a reverse shell on our target. however, soon, you're 30 tabs deep in some random blog posts trying to find out the syntax for that *one command* you know you should've memorized by now but couldn't be bothered to. you give up, head over to pentestmonkey or read through your old notes in an attempt to find that elusive command, and finally, after the motherboard on your target has corroded because of how long it's been, you finally find it; swearing thereon to remember that command so you never forget it again. 

https://user-images.githubusercontent.com/59679082/168722637-88da267c-6d73-414f-8f56-8dc8c56ba6b8.mp4

> okay, yes. that's *quite* the exaggeration, but it's really annoying! anyways, inumaki will make it so that you can just type in the language you need a shell for, and it will spit out the most common ones used in CTFs! 

## ⚡ disclaimer! 
this tool generates reverse shell commands. however, keep in mind that obfuscation does not exist yet. OPSec wise, this tool is the equivalent of running head first into a wall made completely out of megaphones announcing your every move. speaking of reverse shells...

- DO NOT use these shells, or *any* commands such as these on hosts that you do not have EXPLICIT WRITTEN permission to do so.
- the author of inumaki! will not be held responsible if you decide to use this against someone you don't have permission to attack. be smart, guys.
- this tool is going to be an evergrowing project, please report any bugs, issues, etc and I'll try my absolute best to get the issues resolved. this is my first official project so i *am* still learning, but hopefully i can keep up.

## ⭐ installation
```
git clone https://github.com/cr-0w/inumaki.git && cd inumaki
python3 -m pip install -r requirements.txt
chmod +x inumaki
./inumaki
```
---
## to-do 📑
- create support for user-supplied arguments
- add more shells/languages
- add an auto listener initializer for shells like nc, python, etc.
- obfuscated shells? 
