# diy-home-surveillance
###dropbox-upload branch
DIY webcam-driven home surveillance system

Copyright (C) 2015  Gabriele Musco

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.

#Installation instructions for Linux

- git clone this repository
- make sure you have qt, espeak and fswebcam installed in your system
- also make sure you have a functioning webcam since it's the one key part of this software
- cd into the project root folder
- run the following commands:

  qmake imagecompare-qt

  make

- configure dropbox-uploader, a module by @andreafabrizi, by following his readme in his repo: <https://github.com/andreafabrizi/Dropbox-Uploader>
- finally make sure "monitor" has execution permissions (chmod +x monitor)

#Usage

You can launch the program by executing "monitor" in a terminal.
It will start monitoring everything your webcam sees and will repeatedly upload every intruder picture it takes to dropbox and changes the timer between pictures to 3 seconds.
When the intruder gets out, the timer is set back to 10 seconds and pictures are no longer uploaded.

#Notes

I started this project as a hobby, as now I don't plan on doing anything more with it.
I am not responsable for the use you may make of it.
Also, making it open source is a key part of the project, since you can adapt it to your specific needs and let it do whatever you want it to.
