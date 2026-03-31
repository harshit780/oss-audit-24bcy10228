# Open Source Audit Capstone Project

*Student Name:* HARSHIT VERMA  
*Registration/Roll Number:* 24BCY10228
*Chosen Software:* Git  

## Project Overview
This repository contains the practical shell scripting component of "The Open Source Audit" capstone project[cite: 4, 90]. The project explores the philosophy, licensing, and Linux footprint of the open-source version control system, *Git*. Alongside a comprehensive written report, the five shell scripts in this repository demonstrate practical Linux command-line skills and automation[cite: 14, 15].

## Dependencies
To run these scripts successfully, your system must meet the following requirements:
* A Linux environment (Ubuntu via Windows Subsystem for Linux was used for testing).
* bash shell environment.
* Standard GNU core utilities (awk, grep, df, cut, etc.).
* git must be installed.
* Administrative (sudo) privileges may be required to read certain system log files.

## Execution Instructions
Before running any scripts, ensure they have execution permissions. Navigate to the repository directory in your terminal and run:
chmod +x *.sh

---

##Script Descriptions and Usage 

### Script 1: System Identity Report (script1.sh)
* *Description:* Acts as a welcome screen for the Linux environment.It displays the Linux distribution name, kernel version, current logged-in user, system uptime, the current date, and a message regarding the OS's open-source license[cite: 94, 95, 96, 97, 98].
* *How to run:*
  ./script1.sh

### Script 2: FOSS Package Inspector (script2.sh)
* *Description:* Checks if the chosen software (Git) is installed on the system.It retrieves the version information and utilizes a case statement to print a short philosophical description of the software based on its package name[cite: 126].
* *How to run:*
  ./script2.sh

### Script 3: Disk and Permission Auditor (script3.sh)
* *Description:* Loops through a predefined list of important system directories (e.g., /etc, /var/log, /home) to audit them. It reports the disk space each directory uses, alongside its owner and permission string[cite: 146, 147].
* *How to run:*
  ./script3.sh

### Script 4: Log File Analyzer (script4.sh)
* *Description:* Reads a specified system log file line by line. It counts the occurrences of a specific keyword and prints a summary statement of how many times that keyword appeared[cite: 164].
* *How to run:*
  Run with the default keyword ("error"):
  ./script4.sh /var/log/syslog (Note: Ubuntu uses syslog instead of messages)
  Run with a custom keyword (e.g., "warning"):
  ./script4.sh /var/log/syslog warning

### Script 5: Open Source Manifesto Generator (script5.sh)
* *Description:* An interactive script that asks the user three questions regarding their views on open-source tools and freedom. It dynamically concatenates the responses into a personalized "manifesto" paragraph and saves the output to a .txt file[cite: 186].
* *How to run:*
  ./script5.sh
