ansible-pulseaudio
==================

This is a simple ansible role which offers the following features:

* create a user ``multimedia``, with it’s own home and group
* configure that user such that it always has a user session
* run a pulseaudio in that user session
* make that pulseaudio offer network services

Quirks
------

* Everything is hardcoded (I accept PRs to change that!)
* Upon change of any configuration, the pulseaudio daemon is not restarted or
  anything. I don’t know how to fix this (it runs in a user systemd), PRs
  appreciated.

License and attributions
------------------------

It is made for my own use, so no warranties or anything. It works on my Debian
8 deployment. Feel free to use this for your own configuration or make pull
requests to make it more generic. See the LICENSE file for copying information
(spoiler: GPLv3).

    This ansible role is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

This role was made on basis of a [holo][0] package made by
[Stefan Majewsky][1], which fulfills about the same purpose. Conversion to
ansible done by me.

   [0]: https://github.com/majewsky/holo
   [1]: https://github.com/majewsky
