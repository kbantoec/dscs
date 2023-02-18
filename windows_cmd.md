# Windows CMD commands

| Command | Description |
| -- | -- |
| `chkdsk /f` | Goes through your disk and checks if there are any errors and fixes them. Needs restart. |
| `powershell -Command "start-process cmd -verb runas"`| Open cmd as admin |
| `ipconfig` | All your IP information. |
| `ipconfig /all` | Shows more information like DSN server, etc. |
| `ipconfig /displaydns` | |
| `ipconfig /displaydns \| findstr DNS` |  |
| `ipconfig /displaydns \| clip` | |
| `ipconfig /release` | Delete IP address |
| `ipconfig /renew` | Create a new IP address (will renew every single interface on your computer) |
| `ipconfig /flushdns` | Delete DNS caches on your computer (to remove staled DNS entries) |
| `getmac /v` | |
| `powercfg /batteryreport` | |
| `powercfg /energy` | |
| `netstat` | What is connected to your computer and what you are connected to |
| `netstat -af` | Shows what ports are currently open |
| `netstat -o` | ID for your connections |
| `route print` | Prints the route table |
| `shutdown` | Shut down your computer |

## Videos
* [40 Windows Commands you NEED to know (in 10 Minutes)](https://www.youtube.com/watch?v=Jfvg3CS1X3A)