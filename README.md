# System-Utilization

'memory_host' can monitor the memory usage of the host-machine/virtual-machine. It makes use of ’free’ command for 60 seconds and redirect the command output to a text file. Then sum the required column values from the text file using ’awk’ command and calculate the memory usage (%) per minute.

'cpu_host' can monitor the cpu usage of the host-machine/virtual-machine. It makes use of /proc/stat command for 60 seconds and redirect the command output to a text file. Then sum the required column values from the text file using ’awk’ command and calculate the cpu utilization (%) per minute.

'cpu_host_process' can monitor the cpu usage of a process running on a host-machine/virtual-machine. The script is written to monitor the cpu usage of the Virtual Box VM process running on host. It makes use of /proc/<\pid of the process>/stat for 60 seconds and redirect the command output to a text file. Then sum the required column values from the text file using ’awk’ command and calculate the cpu utilization (%) per minute. U_server_5 is the Virtual Box process name, for which the cpu utilization (%) per minute is desired to calculate. vbox.txt is the file name to which the output is redirected. 
Note: Change the name U_server_5 to the process which the cpu utilization (%) per minute is desired to calculate. However, changing the file name vbox.txt is optional.
