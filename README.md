# PS4_db_Rebuilder_EXT

Ps4 built-in database rebuilder has the tendency to remove fpkg from the database. This will repopulate the database with them!

This repository is a modification of the aizenar repository (https://github.com/aizenar/PS4_db_Rebuilder_EXT)

## Requirement

- Python (3.0+)

## Instructions

1) Downdload a release.
2) Start FTP server on the PS4
3) Run the python script through terminal/cmdline:
	
	| Version | Command |
	|--|--|
	| 5.05 | `python3 fix_db.py [PS4_IP] --port [PS4_FTP_PORT] --fw 5.05` |
	| 6.72 - 9.00 | `python3 fix_db.py [PS4_IP] --port [PS4_FTP_PORT] --fw 6.72` |
    | 11.00 | `python3 fix_db.py [PS4_IP] --port [PS4_FTP_PORT]` |

4) Wait for the script to finish, then logout of the PS4 user without closing the browser

5) Log back in and all your games should be there again

Note: For 11.00 you still need to use wifi you cant use pi-pwn for FTP.

## Changes

1) Original Repo https://github.com/aizenar/PS4_db_Rebuilder_EXT
2) Update fix_db.py so now it supports 11.00 firmware.
