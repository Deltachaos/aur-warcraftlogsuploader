# AUR WarcraftLogsUploader Daily Build

This repository provides an automated daily build for updating the Arch Linux AUR package `warcraftlogsuploader`. It fetches the latest release from the official `RPGLogs/Uploaders-warcraftlogs` GitHub repository and updates the package accordingly.

## About

The `warcraftlogsuploader` is a tool for uploading logs to [WarcraftLogs](https://warcraftlogs.com/), allowing World of Warcraft players to share and analyze their raid and dungeon performance. This automated build ensures that the latest release of the uploader is always available on the Arch User Repository (AUR) for Arch Linux users.

The AUR package is available at:  
[warcraftlogsuploader on AUR](https://aur.archlinux.org/packages/warcraftlogsuploader)

## Features

- **Automated daily build**: Automatically fetches the latest release of `Uploaders-warcraftlogs` from the official GitHub repository.
- **Updates the AUR package**: Ensures the `warcraftlogsuploader` package on the Arch Linux AUR stays up to date with the latest features and bug fixes.
- **Easy installation**: Use `yay` or any AUR helper to install and update the package.

## Installation

To install `warcraftlogsuploader` on Arch Linux, use an AUR helper like `yay`:

```bash
yay -S warcraftlogsuploader
```

Alternatively, you can manually install the package from the AUR by downloading the PKGBUILD and running:

```bash
git clone https://aur.archlinux.org/cgit/aur.git
cd aur
makepkg -si
```

## Automatic Updates

This repository automatically checks for the latest release from the [RPGLogs/Uploaders-warcraftlogs](https://github.com/RPGLogs/Uploaders-warcraftlogs) repository and ensures that the AUR package is up to date. The update process is run daily to keep the package current with the latest features and bug fixes.

## How It Works

1. The repository pulls the latest release from the official `Uploaders-warcraftlogs` GitHub.
2. It updates updated PKGBUILD file to match the latest version and source hash.
3. It builds the image to ensure it is still working.
4. The updated PKGBUILD is pushed to the AUR package `warcraftlogsuploader`.
5. Arch Linux users can install or update the package to the latest version via the AUR.

## Contributing

Contributions are welcome! If you find any issues or have ideas for improvements, feel free to create an issue or submit a pull request.

## License

The build job is licensed under the MIT License. The [WarcraftLogs](https://warcraftlogs.com/) Software itself is distributed with its own license and this project is not associated with WarcraftLogs in any way.

## Acknowledgments

- [RPGLogs/Uploaders-warcraftlogs](https://github.com/RPGLogs/Uploaders-warcraftlogs) - WarcraftLogs Release Repository.
- [Arch Linux AUR](https://aur.archlinux.org/) - The Arch User Repository.
