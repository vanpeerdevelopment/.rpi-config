# .rpi-config
Readme and Dotfiles for my Raspberry Pi 5

## Installation
1. i18n and l10n
   - Country: Belgium
   - Language: Flemish
   - Timezone: Brussels
   - System language: English
2. user and password
3. WiFi connection
4. chromium

## Raspberry Pi Configuration 
- System > Hostname: rpi
- Interfaces > SSH: enabled
- Network > WiFi: disabled

## raspi-config
These configurations can also be done from te command line
- `ssh -i ~/.ssh/rpi dieter@rpi.local`
- `sudo raspi-config`