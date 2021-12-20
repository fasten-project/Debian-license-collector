# Debian-license-collector

The Debian license collector performs calls to the Debian APIs, re-creating the directories and files structure for every package hosted in the Debian package repository to retrieve license information at a file level.

This code is running on 8 different machines (all running ubuntu 20.04), data scraping the whole set of packages contained in Debian 11, Bullseye (a total of 46 000 packages).
Each machine is pushing the JSONs retrieved on its branch.

The creation of the directory and files structure is the first step above two, required to retrieve license information at the file level. Next, Debian APIs requires the file checksum to perform the second call where the license information can be obtained.
