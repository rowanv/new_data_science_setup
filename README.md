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
```
touch ~/.bash_profile
pico ~/.bash_profile
```

edit it to include the following:
```
export EDITOR=pico
export VISUAL="$EDITOR"
```
- Set up Github and SSH keys

- Install Python via Homebrew so we are not using system Python
```
brew install python
```
Check that we are defaulting to the homebrew version rather than the system python:
```
which python3
which pip3
```
which should point at `/opt/homebrew/bin/python3` and `/opt/homebrew/bin/pip3`, respectively

Let's make sure our Python is up to date
```
brew upgrade python3
```

Convenience utils:
```
brew install tree
```
