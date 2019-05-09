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

# Coding style
There is no best coding style, everyone prefers something else. I will add some examples for various languages later, but for now I would like to point out the important stuff:
* Every project should follow some coding style for each programming language it contains
* This project style should be adhered to within whole project and shouldn't be mixed with any other styles, the code should be consistent with the rest of code base
* If anything you write is not obvious put comments there and explain your logic. If other people don't understand your logic, they will change your code and that may lead to disaster. Putting comments that explain your thinking, will avoid these disasters.

# Documentation
* Undocumented code is just a bug waiting for removal. If anything is not documented, it shouldn't exist. Every single API and feature needs to be documented somehow.
* Nobody cares about your code if it's not documented.
* **Every documentation needs to contain examples. If it doesn't contain examples, it's not a documentation, it's garbage.**

# Testing and optimization
* Test and compile your code before you commit it
* Try to run (or even better - develop) your software using very slow old computer, with slow CPU and little RAM. That's what most of the planet has. Users have worse computers than programmers. If your software run slow on that kind of computer, people will hate it. Optimize for average hardware.
* Use unit tests if you can - they will make your life easier, continuous integration and unit tests are important.
