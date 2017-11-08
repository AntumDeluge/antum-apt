## Debian/APT Repository for AntumDeluge's Software Packages

### Using this repository:
Add this repository to your system:
1. Add the following line to your */etc/apt/sources.list* file:
  ```
  deb https://raw.githubusercontent.com/AntumDeluge/apt/master <distribution> main
  ```

  *&lt;distribution&gt;* is the name of your Debian/Ubuntu distribution (e.g. "xenial", "yakkety", etc.). Alternatively, you can just use "stable" as currently, all packages are the same for all distributions.

2. Now update APT's cache:
  ```
  $ sudo apt update
  ```

Add the public GPG key to your system:
- There are multiple options for adding the public key
  - Using the APT package manager (after adding repository & updating APT's cache):

    ```
    $ sudo apt install antum-pubkey-installer
    ```
  - Using wget:

    ```
    $ wget -O- https://raw.githubusercontent.com/AntumDeluge/apt/master/antum-pub-gpg.key | sudo apt-key add -
    ```
  - Using public key server:

    ```
    $ sudo apt-key adv --no-default-keyring --keyserver keyserver.ubuntu.com --recv-keys F44C290A
    ```

### Included software packages:
- [Debreate][]: Debian package builder ([direct download](https://github.com/AntumDeluge/debreate/releases/latest))
- [Stendhal (no blood)][Stendhal]: Modified version of the Stendhal game client that removes blood settings ([direct download](https://github.com/AntumDeluge/arianne-stendhal/releases/latest))
- stendhal-webstart: Script that launches the Stendhal client from the remote webstart applications (.jnlp)


[Debreate]: https://AntumDeluge.github.io/debreate-web
[Stendhal]: https://stendhalgame.org/
