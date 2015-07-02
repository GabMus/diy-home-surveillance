# diy-home-surveillance
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

- finally make sure "monitor" has execution permissions (chmod +x monitor)

#Usage

You can launch the program by executing "monitor" in a terminal.
It will start monitoring everything your webcam sees and will trigger the "intruder alert" repeated message until it's closed by pressing ctrl+c in the terminal.
At this point the program is stopped and the photo of the intruder is saved in the root folder of the program.

#Notes

I started this project as a hobby, as now I don't plan on doing anything more with it.
I am not responsable for the use you may make of it.
Also, making it open source is a key part of the project, since you can adapt it to your specific needs and let it do whatever you want it to.
