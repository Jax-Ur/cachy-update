# Fork of Cachy-Update (fork of [Arch-Update](https://github.com/Antiz96/arch-update))

<p align="center">
  <img width="460" height="300" src="https://github.com/user-attachments/assets/5782bd11-084a-4ca3-b599-1c322ee11b84">
</p>

## Table of contents

- [Description](#description)
- [Installation](#installation)
- [License](#license)

## Description

Fork of the [Cachy-Update](https://github.com/CachyOS/cachy-update) program with added "update frequency" settings. Current options are:
* Hourly (resets the original)
* Daily, daily from the time this setting is applied and the last time check update was run
* Weekly, 7 days from the time this setting is applied and the last time check update was run
* Monthly, 30 days from the time this setting is applied and the last time check update was run

## Installation

Install required build dependencies:

```bash
sudo pacman -S --asdeps make scdoc bats
```

Download the archive and extract it (alternatively, you can clone this repository with `git`).

To install the modified `cachy-update`, go into the extracted / cloned directory and run the following commands:

```bash
make build
make test
sudo make install
```

Once the installation is complete, you may optionally clean up the directory of files generated during installation by running the following command:

```bash
make clean
```

To uninstall the modified `cachy-update`, go into the extracted / cloned directory and run the following command:

```bash
sudo make uninstall
```

##


## License

Arch-Update is licensed under the [GPL-3.0 license](https://github.com/CachyOS/cachy-update/blob/main/LICENSE) (or any later version of that license).
