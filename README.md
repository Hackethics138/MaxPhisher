# MaxPhisher
A python phishing script for login phishing, image phishing, video phishing and many more
Install primary dependencies (git, python)

    For Debian (Ubuntu, Kali-Linux, Parrot)
        sudo apt install git python3 python3-pip php openssh-client -y
    For Arch (Manjaro)
        sudo pacman -S git python3 python-pip php openssh --noconfirm
    For Redhat(Fedora)
        sudo dnf install git python3 php openssh -y
    For Termux
        pkg install git python3 python-pip php openssh -y

Clone this repository

    https://github.com/Hackethics138/MaxPhisher

Enter the directory

    cd MaxPhisher

Install all modules

    pip3 install -r files/requirements.txt --break-system-packages

Run the tool

    python3 maxphisher.py

Or, directly run

wget https://raw.githubusercontent.com/Hackethics138/MaxPhisher/main/maxphisher.py && python3 maxphisher.py
Pip

    pip3 install maxphisher [For Termux]
    sudo pip3 install maxphisher --break-system-packages [For Linux]
    maxphisher

Docker

    sudo docker pull kasroudra/maxphisher
    sudo docker run --rm -it kasroudra/maxphisher
    sudo docker cp $(sudo docker ps | grep maxphisher | awk '{print $1}'):/root/Media media [Run this on another terminal to copy received files from docker to media folder while keeping the container running]
usage: maxphisher.py [-h] [-p PORT] [-t TYPE] [-o OPTION]
                     [-T TUNNELER] [-r REGION] [-S SUBDOMAIN]
                     [-d DIRECTORY] [-f FEST] [-i YTID] [-u URL]
                     [-s DURATION] [-m MODE] [-e TROUBLESHOOT]
                     [--nokey] [--noupdate]

options:
  -h, --help            show this help message and exit
  -p PORT, --port PORT  MaxPhisher's server port [Default : 8080]
  -t TYPE, --type TYPE  MaxPhisher's phishing type index [Default :
                        null]
  -o OPTION, --option OPTION
                        MaxPhisher's template index [ Default : null ]
  -T TUNNELER, --tunneler TUNNELER
                        Tunneler to be chosen while url shortening
                        [Default : Cloudflared]
  -r REGION, --region REGION
                        Region for loclx [Default: auto]
  -S SUBDOMAIN, --subdomain SUBDOMAIN
                        Subdomain for loclx [Pro Account]
                        (Default: null)
  -d DIRECTORY, --directory DIRECTORY
                        Directory where media files will be saved
                        [Default : /sdcard/Media]
  -f FEST, --fest FEST  Festival name for fest template [Default:
                        Birthday]
  -i YTID, --ytid YTID  Youtube video ID for yttv template [Default :
                        6hHmkInZkMQ (NASA Video)]
  -u URL, --url URL     Redirection url for ip-tracking or login
                        phishing [Default : null]
  -s DURATION, --duration DURATION
                        Media duration while capturing [Default :
                        5000(ms)]
  -m MODE, --mode MODE  Mode of MaxPhisher [Default: normal]
  -e TROUBLESHOOT, --troubleshoot TROUBLESHOOT
                        Troubleshoot a tunneler [Default: null]
  --nokey               Use localtunnel without ssh key [Default:
                        False]
  --noupdate            Skip update checking [Default : False]
