## Debian/APT Repository for AntumDeluge's Software Packages

### Using this repository:
Add the following line to your */etc/apt/sources.list* file:
```
deb https://raw.githubusercontent.com/AntumDeluge/apt/master <distribution> main
```

*&lt;distribution&gt;* is the name of your Debian/Ubuntu distribution (e.g. "xenial", "yakkety", etc.). Alternatively, you can just use "stable" as currently, all packages are the same for all distributions.

Add the public GPG key to your system:
```
$ wget -O- https://raw.githubusercontent.com/AntumDeluge/apt/master/antum-pub-gpg.key | sudo apt-key add -
```

Now update APT's cache:
```
$ sudo apt update
```

### Included software packages:
- [Debreate][]: Debian package builder ([direct download](https://github.com/AntumDeluge/debreate/releases/latest))
- [Stendhal (no blood)][Stendhal]: Modified version of the Stendhal game client that removes blood settings ([direct download](https://github.com/AntumDeluge/arianne-stendhal/releases/latest))


[Debreate]: https://AntumDeluge.github.io/debreate-web
[Stendhal]: https://stendhalgame.org/
