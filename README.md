Intro
=====

This repository contains playlists from KCRW. All data is retrieved from KCRW's site, http://www.kcrw.com/playlists. The goal is to provide the playlists in a convenient form for the purpose of analysis.

Folder Structure
================

At the top level, there are (or soon will be) two folders, `simulcast` and `eclectic24`, each containing the respective playlists for two KCRW stations that play music.

Beneath the top level, the structure is the same: a folder per year, containing the playlist for each day of the year. The file names follow a pattern as well:

	[year]-[month]-[day]-[simulcast,eclectic24].json

File Structure
==============

Each json file containing the daily playlist is, at the top level, a dictionary with the following keys:

- version : The file version. Currently always 1.0
- total : The number of entries in the playlist
- error : Only present if an error occurred that prevented full retrieval of the playlist
- songs : The content returned by KCRW for the playlist query

