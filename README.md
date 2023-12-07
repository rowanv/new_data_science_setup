# new_data_science_setup
A repo for describing a new setup process when getting a new dev Mac


- Install XCode

- Create working directory:
```
$ cd ~/
$ mkdir workspace
$ mkdir venvs
```

- Install Sublime text
- Create the symlink for the command line interface tool `subl`
```
$ ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/.
$ echo $PATH
```

- Make pico the default editor

- Set up Github and SSH keys

- Install Python via Homebrew so we are not using system Python
```
brew install python
```
Link to it in `.bashrc
```
pico .bashrc
alias python=/usr/local/bin/python3
alias pip=/usr/local/bin/pip3
```

Open a new terminal window to make sure the `.bashrc` settings take effect

Double check that the right version of python is being used:
```
which python3
```
which should point at `python3: aliased to /usr/local/bin/python3
