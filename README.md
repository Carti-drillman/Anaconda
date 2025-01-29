# Anaconda 1.3

Anaconda 1.3 have some new features. Now it has System syntaxes or OS devlopment syntaxes.

# File Operations

`create_file "source"` : Creates an empty file.

`write_file "source"` : Writes text to a file.

`read_file "source"` : Reads and prints file contents

`delete_file "source"` : Deletes a file

# Process Management

`start_process "command"` : Starts a system process.

`stop_process "command"` : Stops a process by name.

`list_processs` : Lists all running processes.

# Memory Management

`allocate_memory` : Allocates memory.

`free_memory` : Frees memory.

# Networking

`open_port port_number` : Opens a port.

`send_data "data" "host port` : Sends data to a host via a port.

`receive_data` : Receives data from a port.

`close_port` : Closes the network socket.

# Example code

`example.ana`

```python
print "Starting system initialization..."
create_file "log.txt"
write_file "log.txt" "System initialized."

start_process "shell"
list_processes
get_os_info

if get_cpu_info > 2:
    print "Sufficient CPU cores available."

stop_process "shell"
delete_file "log.txt"
print "System shutdown completed."
```

Don't forget to contact us at mmbkmcgamming2014@gmail.com!
