# condor-tools
Various tools that enhance your condor experience.

### Getting Started
To add condor_shell to your `PATH` simply:
```
source enable
```

### `condor_shell`
Request an interactive job from condor.

You can specify the machine you would like to request:
```
condor_shell --machine fix
```

You can also specify whole machine jobs if necessary:
```
condor_shell --whole
```

These can also be combined:
```
condor_shell --machine allagash --whole
```


By default, `condor_shell` will start the condor job in the same directory it is executed from.

You can specify the directory you'd like to start in instead:
```
condor_shell -C /home/me/my_dir
condor_shell -C ../other_dir
```

Or you can be placed in the usual condor limbo:
```
condor_shell --nwd
```

### `condor_usage`
Query machines currently in use and their users.

With no arguments, this will give you information about all running jobs (and their user).
```
condor_usage
```

Or, you can specify the machine you want to inspect:
```
condor_usage --machine allagash
```
