# MARS: Myhat2you's Auto-Ricing Script

**MARS** is an automated ricing script for Arch-based Linux distributions, inspired by Luke Smith's LARBS. 
This script installs and configures a fully-featured Linux desktop environment, customized with Myhat2you's dotfiles and preferences.

---

## Features
- **Automated Installation**: Installs required packages, dotfiles, and desktop environment.
- **Custom Configuration**: Includes my personal configurations for tools like Neovim, Librewolf, and Zsh.
- **Privacy & Usability Enhancements**:
  - Firefox/Librewolf ricing with Arkenfox user.js and addons.
  - Touchpad tap-to-click configuration.
- **Cronjobs**: Automates news updates, email sync, and system maintenance tasks.
- **System Setup**: Handles user creation, shell setup, keyring updates, and more.

---

## Prerequisites
- A clean Arch-based Linux installation.
- Network connectivity.
- Run as the `root` user.

---

## Usage

1. **Download the script**:
   ```bash
   git clone https://github.com/myhat2you/MARS.git
   cd MARS
   chmod +x mars.sh
   ```

2. **Run the script**:
   ```bash
   ./mars.sh
   ```

3. **Follow the prompts**:
   - Provide a username and password.
   - Confirm user overwrites if necessary.
   - Sit back and let the script do the rest.

---

## Key Components
- **Dotfiles Repository**: [myhat2you/rice](https://github.com/myhat2you/rice)
- **Program List**: [progs.csv](https://github.com/myhat2you/MARS/static/progs.csv)
- **AUR Helper**: `yay` (can be replaced if needed).

---

## Customization
- Edit variables at the top of the script to customize:
  - `dotfilesrepo`: Change the dotfiles source repository.
  - `progsfile`: Modify the CSV file that lists all programs to install.
  - `aurhelper`: Use a different AUR helper.
  - `repobranch`: Specify a branch for the dotfiles.

---

## Troubleshooting
- Ensure `pacman` is up-to-date and keyrings are refreshed:
  ```bash
  pacman -Syu
  pacman -S archlinux-keyring
  ```
- Run the script in a supported environment (Arch or Arch-based distributions).
- Check the script logs if any step fails.

---

## Contributions
Feel free to fork, modify, or contribute improvements via pull requests to the [GitHub repository](https://github.com/myhat2you/MARS).

---

## License
This project is distributed under the MIT License. See the LICENSE file for details.

---

### Credits
- **Original Inspiration**: [Luke Smith's LARBS](https://larbs.xyz)
- **Modified and Maintained by**: J Talbot <talbot@hackersec.xyz>
