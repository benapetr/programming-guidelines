# Programming Guidelines
Because there is too much shit software and bad programmers out there, I created this to help people write good software. Feel free to improve this with pull requests.

# Error messages
Error messages **must** be verbose and clear. They need to say exactly what went wrong and if possible, why. If you don't want to show too much details so that you don't confuse average users, you should at least add a pointer for advanced users (error details can be found in /var/log/my_program). If you don't generate verbose error messages **your software sucks**.
## Good
* Error: unable to write to file /tmp/something.dat: permission denied
* Error: unable to write to file /tmp/something.dat: not enough space left to write to device
* Error: connection to server.org on port 545 TCP failed: socket closed
## Bad
* Error
* This is error, that's all we know
* Something wrong happened
