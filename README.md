# kali-vega-sandbox
~~~~
>vagrant up vg-kali-02

>vagrant ssh vg-kali-02
Linux vg-kali-02 5.10.0-kali3-amd64 #1 SMP Debian 5.10.13-1kali1 (2021-02-08) x86_64

The programs included with the Kali GNU/Linux system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Kali GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
permitted by applicable law.
┏━(Message from Kali developers)
┃
┃ We have kept /usr/bin/python pointing to Python 2 for backwards
┃ compatibility. Learn how to change this and avoid this message:
┃ ⇒ https://www.kali.org/docs/general-use/python3-transition/
┃
┗━(Run “touch ~/.hushlogin” to hide this message)
┌──(vagrant㉿vg-kali-02)-[~]
└─$

>vagrant destroy -f vg-kali-02

~~~~
~~~~
>vagrant up vg-kali-04 vg-kali-05

>vagrant ssh vg-kali-05
$ ping -c 2 192.168.50.5
PING 192.168.50.5 (192.168.50.5) 56(84) bytes of data.
64 bytes from 192.168.50.5: icmp_seq=1 ttl=64 time=0.632 ms
64 bytes from 192.168.50.5: icmp_seq=2 ttl=64 time=0.466 ms

$ ping -c 2 vg-kali-04
PING vg-kali-04.local (192.168.50.5) 56(84) bytes of data.
64 bytes from vg-kali-04.local (192.168.50.5): icmp_seq=1 ttl=64 time=0.685 ms
64 bytes from vg-kali-04.local (192.168.50.5): icmp_seq=2 ttl=64 time=0.667 ms

>vagrant destroy -f vg-kali-04 vg-kali-05
~~~~
~~~~
>vagrant ssh vg-kali-02
sudo docker-compose --file dockerfiles/kalilinux/docker-compose-kali.yml up -d
sudo docker-compose --file dockerfiles/kalilinux/docker-compose-kali.yml ps
sudo docker-compose --file dockerfiles/kalilinux/docker-compose-kali.yml stop
sudo docker-compose --file dockerfiles/kalilinux/docker-compose-kali.yml down -v

sudo docker exec --tty --interactive kali /bin/bash
sudo docker network ls   

https://github.com/githubfoam/cyberrange-sandbox

~~~~
~~~~
GUI interface
username/password vagrant/vagrant

https://app.vagrantup.com/kalilinux/boxes/rolling
~~~~
~~~~
https://hub.docker.com/u/kalilinux

https://hub.docker.com/r/kalilinux/kali-rolling
~~~~
