# Windows System Resource Usage Monitor (SRUM) 

Contains a wealth of information about all the activities that occur on your machine. Some of this information is visible from the "APP HISTORY" tab on the task manager, but a vast amount of detail collected is not displayed via the GUI. 

It keeps the names and paths of every application that executes on your system even the ones the attackers deleted. It records the user's SID that execute the program so we knew the attacker used a temporary account that the administrators clean up deleted. It records then names of all of the networks you have connected to and how long you were connected. It also records application battery usage, CPU time broken down by foreground and background time, how many bytes were written and read from the hard drive by the application and much more. 

**Location:**

- \Windows\System32\sru\ directory in a file named SRUDB.DAT.

The file is in the Windows ESE (Extensible Storage Engine) database format. 

**How to obtain that file?**

1. FTK imager, add evidence (logical driver) and copy this file to desire location. 
2. Mount Shadow Volume and obtain older version of this file.

**Tools:**

- https://github.com/MarkBaggett/srum-dump
