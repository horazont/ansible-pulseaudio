ansible-pulseaudio
==================

This is a simple ansible role which offers the following features:

* create a user ``multimedia``, with it’s own home and group
* configure that user such that it always has a user session
* run a pulseaudio in that user session
* make that pulseaudio offer network services

It is made for my own use, so no warranties or anything. It works on my Debian
8 deployment. Feel free to use this for your own configuration or make pull
requests to make it more generic. See the LICENSE file for copying information
(spoiler: GPLv3).

This role was made on basis of a [holo][0] package made by
[Stefan Majewsky][1], which fulfills about the same purpose.

   [0]: https://github.com/majewsky/holo
   [1]: https://github.com/majewsky
