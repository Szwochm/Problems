# The Problem: Portable Progamming Enviroment

1. I am taking classes that need the following IDEs

    Intellij, Android Studio, Eclipse, and Visual Code.

2. I am trying to use minimal resources as I work on school computers, personal computers, and my laptop. I want to put the enviroment on a harddrive that I can just plug n play on any device

## Proposed Solution \#1 Docker Containers

## Questions to answer:

### Do docker containers use less resources than hosting a vm?

Yes, according to [1](https://www.backblaze.com/blog/vm-vs-containers/), the following is a comparison of docker vs VMs. **Note on Windows, docker uses [WSL2 or hyper-v.](https://docs.docker.com/desktop/install/windows-install/) 


![image](https://user-images.githubusercontent.com/1501624/213533002-a7335042-6c52-42bd-bf0a-0d4a4007957e.png)

### Is the Windows docker still faster than hosting a VM

No answer yet. Annecdotally people on [dockers forums](https://docs.docker.com/search/?q=windows%20slow) complained that windows is 2x slower on docker than on a hosted vm. Something to look into later if I have performance issues.

### Can I run the same containers on both Windows and Linux?

I believe so. According to [dockers documentation](https://docs.docker.com/engine/faq/#:~:text=You%20can%20run%20both%20Linux,on%20Linux%2C%20Windows%20and%20macOS.) "You can run both Linux and Windows programs and executables in Docker containers. The Docker platform runs natively on Linux (on x86-64, ARM and many other CPU architectures) and on Windows (x86-64)."  This seems to imply some sort of cross-compatibility but doesn't exactly answer the question.

### Is there any problems associated with running Programming Enviroments on containers?

There are some security concerns with libraries, and the lack of isolation docker provides vs a VM

### Is there docker container support for the IDEs specified?

No answer yet.

### Can I run this on school computers? Docker on Windows needs virtualization. Not sure if the school computers have docker running.


## Prototype - Lets try it with the most supported IDE, see how its goes.

1. Does it work on both my laptop and desktop?

2. Does it work on both linux and desktop?

3. Can I plug this into any computer with docker and it works reasonably well?




## Proposed Solution \#2 Run Environment on Bootable drives or as a VHD

Someone recommended using [IODD ST400](https://www.youtube.com/watch?v=ZSywLblIYa0)

## Problems

### I know in the past, using a bootable usb had issues connecting to the internet because different workstations have different hardware and drivers associated. Is this still an issue?



## References

[IODD ST400](https://www.youtube.com/watch?v=ZSywLblIYa0)

[Docker Vs VM -backblaze.com](https://www.backblaze.com/blog/vm-vs-containers/)

[Docker Windows Install](https://docs.docker.com/desktop/install/windows-install/)


