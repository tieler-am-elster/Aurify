# Aurify
Aurify is a minimal **AUR helper** written in Bash designed for bypassing the main AUR repo. Instead, it uses the AUR GitHub mirror for safety and reliability.
This script was written for one specific purpose: to bypass main AUR repo downtime while maintaining simplicity and ease of use.
> [!WARNING]
> Note: Aurify is minimal and not secure by design. PKGBUILDs are sourced directly, without interactive confirmation. It’s intended as an emergency fallback during AUR downtime — not as a replacement for yay/paru in everyday use (until some security features would be added).

## Features
- Installing AUR packages directly from the GitHub mirror
- Automatic dependency resolution (AUR + official repos)
- Colored output for readability and accessibility
- Building in a safe, temporary directory (no clutter)

## Installation
> [!WARNING]
> The script depends on git and base-devel, ensure those packages are installed before proceeding.

To install type in the terminal:
`sudo curl -fsSL https://raw.githubusercontent.com/tieler-am-elster/Aurify/refs/heads/master/aurify -o /usr/bin/aurify && sudo chmod +x /usr/bin/aurify`

## Usage
To install/update a package:
```bash
aurify <package-name>
```
