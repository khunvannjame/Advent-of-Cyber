# Machine : Linux CLI - Shells Bells

# Method of Solve
* Switch the directory by running cd Guides. You will appear at /home/mcskidy/Guides.
* Run the ls command again to list the content of the guides directory (it will be empty).
* View the directory again by running `ls -la`. The -a flag shows the hidden files. The `-l` flag shows the additional details, such as file permissions and file owner.
* Read the hidden guide by running `cat .guide.txt`. Don't forget the leading dot.
* Navigate to the logs directory with `cd /var/log` and explore its content with `ls`.
* Run `grep "Failed password" auth.log` to look for the failed logins inside the `auth.log`.
* Run `find /home/socmas -name *egg*` to search for "eggs" in the socmas home directory.
* File found `/home/socmas/2025/eggstrike.sh`.
* Note that find is a powerful command.
* Analyzing the eggstrike.sh
* `cat eggstrike.sh` 

```
# Eggstrike v0.3
# © 2025, Sir Carrotbane, HopSec
cat wishlist.txt | sort | uniq > /tmp/dump.txt
rm wishlist.txt && echo "Chistmas is fading..."
mv eastmas.txt wishlist.txt && echo "EASTMAS is invading!
```

  1. The lines starting with # are just comments and are not the actual commands.
  2. The cat wishlist.txt | sort | uniq lists unique items from the wishlist.txt.
  3. The command then sends the output (unique orders) to the /tmp/dump.txt file.
  4. The rm wishlist.txt deletes the wishlist file (containing Christmas wishes).
  5. The mv eastmas.txt wishlist.txt replaces the original file with eastmas.txt.

* Server has benn breach 
* See how Sir Carrotbane replaced the wishlist by visiting `http://10.64.191.46:8080` 
* check the usernames and hashed password of users by `cat /etc/shadow` you need tobe root user to execute that command
* Normal user type `cat .bash_history` 
* Root user type `history` to view the saved commands in hidden history.

# Flag
* ### THM{learning-linux-cli}
* ### THM{sir-carrotbane-attacks}
* ### THM{until-we-meet-again}

# Command 
* ls / ll = List Directory (Files)
* echo = To display back
* cat = To view the contents in the files
* pwd = Print Work Directory
* ls -a = Show the hidden files.
* ls -l = Show the additional details (file permission, file owner)
* `/var/log` = a Linux directory where all security events (logs) are stored
* grep = a command to look for a specific text inside a file
* find = a command that searches for files with specific parameters, such as -name
* `.sh` = Shell Script
* Pipe symbol (|) = Send the output from the first command to the second
* Output redirect (>/>>) = Use > to overwrite a file, and >> to append to the end
* Double ampersand (&&) = Run the second command if the first was successful
* `uptime` to see how much time your system is running
* `ip addr` to check your IP address
* `ps aux` to list all processes
* check the usernames and hashed passwords of users by running `cat /etc/shadow` (need root permission)
* `whoami` to verify your current user
* `sudo su` Switch to the root user
* To view every saved command that run in hidden history file `cat .bash_history`
In root user type `history`
