## inumaki! 🦴
**inumaki!** is a command-line tool which helps remove the tedium of common capture-the-flag 'shell searching'. it's also my first official project! we've all been there; a bit of time has passed after our enumeration and we're finally ready to send a reverse shell on our target. however, you're soon 30 tabs deep into some random blog post trying to find out the syntax for that command you know you should've memorized by now but couldn't be bothered to. you give up, head over to pentestmonkey or read through your old notes in an attempt to find that elusive command, and finally, after the motherboard on your target has corroded because of how long it's been, you finally find it; swearing thereon to remember that command so you never forget it again. 

Okay, yes. That's *quite* the exaggeration, but it's really annoying! Anyways, inumaki will make it so that you can just type in the language you need a shell for, and it will spit out the most common ones used in CTFs! 

## installation
```
git clone https://github.com/cr-0w/inumaki.git && cd inumaki
python3 -m pip install -r requirements.txt
chmod +x inumaki
```

## usage
```
./inumaki
```
