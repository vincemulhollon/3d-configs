# 3d-configs
These are standard configs for my 3d printing workflow on freebsd

cd ~/Dropbox/printrbot

git clone https://github.com/vincemulhollon/3d-configs configs

(I have Dropbox on freebsd because I run openafs home dirs, and have dropbox running on some legacy box)

makefile.standard includes some installation commentary for various 3d printing software on FreeBSD

slic3r.ini.standard is for my printrbot simple metal with heated bed printing 1.75mm PLA on kapton

My typical workflow involves editing openscad designs in emacs, then a simple makefile processes them down to stl and then gcode while mixing global standard settings (printer geometry, etc) with project settings (infill, etc).  Finally I use a web browser or octocmd to upload to my octoprint running on the octopi distro on a raspberry pi connected to the printrbot.

So in summary, I edit openscad code in emacs where I hit meta-x compile, and a minute later I click print on the octoprint web interface.

