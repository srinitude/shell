# Shell

<img src="https://github.com/srinitude/simple_shell/blob/master/hsh.png" style="height:15%;width:15%" />

## Welcome
Thanks for happening upon our project, Shell! Shell was inspired by Ken Thompson and the initial UNIX Shell. Felicia and I started development with the goal of creating a very basic shell that has similar functionality to the Thompson and bash shells, but we're each planning on forking this current project and developing our own individual sets of additional, domain-specific functionality that you will not be able to find on many of the shells that are currently out there in the ether. However, before forking to work on our own separate projects, we'll be adding more features and bug fixes to the current repo in order to realize to a "Minimum Viable Shell" (MVS).

For those interested in what happens when a typical shell executes a command typed by the user in the terminal, check out this [blog post](https://medium.com/@feliciaSWE/linux-command-ls-c-930cf1d7d8a6).

## Table of Contents
* [Requirements](#requirements)
* [Installation](#installation)
* [Usage](#usage)
* [Commands](#commands)
* [Roadmap](#roadmap)
* [Testing](#testing)
* [Credits](#credits)
* [License](#license)

## Requirements
* Ubuntu 14.04 LTS
* gcc 4.8.4 (-Wall, -Werror, -Wextra, and -pedantic flags)

## Installation
```sh
gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
```

## Usage
Commands are currently executed just like they are in sh, bash, and other common shells.

To start Simple Shell in interactive mode, run the command below:
```sh
./hsh
```

To start Simple Shell in non-interactive mode, `echo` the command or `cat` the pseudo-random file you want to run and pipe the standard output into Simple Shell:
```sh
echo "ls -l" | ./hsh
```

## Commands
The commands that you can use right now with Shell are indicated with a checkmark. The ones that aren't are left unchecked. Of course, the builtins provided aren't the only builtins we plan on implementing. The usage of these commands are similar to that of sh, bash, and many of the most commonly-used shells.

* Builtins
  - [x] exit
  - [x] env
  - [x] pwd
  - [ ] cd
  - [ ] setenv
  - [ ] unsetenv
  - [ ] help
  - [ ] history
* $PATH Commands

## Roadmap
We may currently have a functional shell where you can use several builtins and commands found in the directories listed in the PATH environment variable, but we are definitely not yet done with our "Minimum Viable Shell." Below are the tasks we would like to accomplish before forking this project and creating our own domain-specific shells.

- [x] Fix current memory leaks
- [ ] Add better memory management
- [ ] Handle commands separator (`;`)
- [ ] Handle logical operators (`||`, `&&`)
- [ ] Handle aliases
- [ ] Handle variable replacement
- [ ] Handle the `$?` variable
- [ ] Handle the `$$` variable
- [ ] Handle comments
- [ ] Handle many of the common shell builtins

## Testing
If you as a developer would like to fork our current project and create your own domain-specific shell, feel free to use a [testing suite](https://github.com/srinitude/shellgame) that we created to compare the output and errors of our/your shell with that of sh's.

## Credits
Shell is owned and maintained by Kiren Srinivasan ([@srinitude](https://twitter.com/srinitude)) and Felicia Hsieh ([@feliciahsiehsw](https://twitter.com/feliciahsiehsw)). You can reply to us and to [@holbertonschool](https://twitter.com/holbertonschool) on Twitter for more updates on this project and our forked projects.

## License
Shell is released under the MIT license. See [LICENSE](https://github.com/srinitude/simple_shell/blob/master/LICENSE) for details.
