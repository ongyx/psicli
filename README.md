<p align="center">
  <a href="https://github.com/sn3ksoftware/psilib">psilib</a> &bull;
  <b> psiman </b> &bull;
  <a href="https://github.com/sn3ksoftware/psidex">psidex</a>
</p>

# psiman: The PSIdex package MANager
(formerly [spkg for Libterm](https://github.com/sn3ksoftware/sandpkg/tree/testing))

![GitHub release (latest SemVer including pre-releases)](https://img.shields.io/github/v/release/sn3ksoftware/psiman?include_prereleases&sort=semver)

<img src="https://raw.githubusercontent.com/sn3ksoftware/psiman/master/psiman_logo.png" alt="psiman_logo:Ψ" width="200"/>

Welcome to the repo for psiman, a frontend for psilib that uses the [psidex](https://github.com/sn3ksoftware/psidex) system.

For mobile users, click [here](https://github.com/sn3ksoftware/psilib/wiki) to access the psilib/psiman wiki.

Platforms supported:

| Platform  | Version of psiman(cli-wrapper) |
| --- | --- |
| [Libterm](https://github.com/ColdGrub1384/LibTerm) | v0.1.0 |
| [Pythonista](http://omz-software.com/pythonista/) | v0.1.0 |
| Linux/GNU and *nix | -WIP- |
| Windows | -WIP- |

(More platforms will be added as needed.)

# What’s the point?
I wanted to revive the [Pythonista Script Index](https://github.com/sn3ksoftware/Pythonista-Script-Index) proof of concept
because it would be a waste to not try and complete it as much as possible.
Also, becuase the Pythonista Script Index pushes part of the repo management to the dev, allowing for easier
updating of scripts and modules.

This means that index.json is in one repo, package.json in another and the actual zip containing the package in yet another repo!


I moved psilib to another repository, and the psilib code was abstracted from psiman
so that:
1. psilib can be scripted.
2. psilib can be developed independently of psiman.
3. The psilib code can be reused by other developers more cleanly.

# Dependencies
Python 3.5+ is required as psiman is written in Python3.
The requests library is the only external dependency (preinstalled on Pythonista and Libterm),
so it should work out of the box.
For Pythonista, [StaSh](https://github.com/ywangd/stash) is required to run psiman.
Install with `import requests as r; exec(r.get('https://bit.ly/get-stash').text)`.

# Installation

## Libterm/Pythonista:

If you are on Pythonista, launch a StaSh instance first (launch_stash.py and press the play button).
Download the installer and run it.
```
curl -O https://raw.githubusercontent.com/sn3ksoftware/psilib/master/install.py
python install.py
```

Configuration files are, by default, stored at `~/Documents/.psicfg`.

# P.S
The code from [spkg for Libterm](https://github.com/sn3ksoftware/sandpkg/tree/testing) was _heavily_ modified to use the json-based `psidex` system.
Its original source code, including the psiman package manager, is under the MIT License.
