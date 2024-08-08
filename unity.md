# Unity on Ubuntu 22.04

To install Unity 2021 on Ubuntu 22.04:
- install Unity Hub via apt `sudo apt install unityhub`
- install libssl1

  `echo "deb http://security.ubuntu.com/ubuntu focal-security main" | sudo tee /etc/apt/sources.list.d/focal-security.list`

  `sudo apt-get update`

  `sudo apt-get install libssl1.1`

  `sudo rm /etc/apt/sources.list.d/focal-security.list`

- Unity should be installed in `/opt`
- Set UnityHub script as default app in Browser 
- Add `--no-sandbox` option to launch command in UnityHub script