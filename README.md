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
| Linux (Generic) | -WIP- |
| Windows | -WIP- |

(More platforms will be added as needed.)
# Dependencies
psiman, of course, requires Python 3.5+.
It only requires stlib that comes with Python 3.5+ and the requests library (preinstalled on Pythonista and Libterm), so it should work out of the box.
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
