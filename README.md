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
