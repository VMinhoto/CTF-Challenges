# URL
https://tryhackme.com/room/windowscommandline
# Category
Fundamentals
# Concept
Learning how to work with windows command line
# Method of solve

## Task 1 - Basic system info
* `set` displays the current environment variable settings
* `ver` displays the operating system version number
* `systeminfo` Displays detailed configuration information about a computer and its operating system, including operating system configuration, security information, product ID, and hardware properties (such as RAM, disk space, and network cards)
* * Run `systeminfo`. Answers are `10.0.20348.2655` and `WINSRV2022-CORE`
 
## Task 2 - Netwworking
* `ipconfig` checks your network information. `ipconfig \all` gives more info
* `ping target_name` pings the taget
* `tracert target_name` traces the network route traversed to reach the target
* `nslookup`  looks up a host or domain and returns its IP address
* `netstat` displays current network connections and listening ports
  * -a displays all established connections and listening ports
  * -b shows the program associated with each listening port and established connection
  * -o reveals the process ID (PID) associated with the connection
  * -n uses a numerical form for addresses and port numbers
* The command is `ipconfig \all`
* Use `netstat -abon` to find the ansers `RpcSs` and `TermService`

  ## Task3 - Files management
  * `cd` changes directory. Use standalone to print current directory
  * `dir` list files and directories under this directory. `dir /a` Displays hidden and system files as well. `tree` gives a more visual result.
  * `mkdir` creates a directory. `rmdir` removes a directory
  * `type` prints the content of a file
  * `copy` copies a file
  * `move` moves a file
  * `del` or `erase` deletes a file
  * To solve the challange write `type C:\Treasure\Hunt\flag.txt`
 
  ## Task4 - Task and process manager
  * `tasklist` list the running processes
  * `tasklist /FI "imagename eq sshd.exe"` /FI is used to set the filter image name equals sshd.exe
  * `taskkill /PID target_pid` to kill a process with a PID
 
  ## Task 5
  * `shutdown /r`
  * `shutdown /a`
