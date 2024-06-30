# SSH

## Login using public private key
1. Generate new keypair: `ssh-keygen -f ~/.ssh/rpi`
2. Copy public key to rpi authorized keys: `ssh-copy-id -i ~/.ssh/rpi.pub dieter@rpi.local`
3. Connect using ssh: `ssh -i ~/.ssh/rpi dieter@rpi.local`

## Disable password login
1. Connect using ssh: `ssh -i ~/.ssh/rpi dieter@rpi.local`
2. Create ssh config file: `sudo touch /etc/ssh/sshd_config.d/disable_password_login.conf`
3. Write config: `sudo nano disable_password_login.conf`
```
ChallengeResponseAuthentication no
PasswordAuthentication no
UsePAM no
PermitRootLogin no
X11Forwarding no
```
4. Restart sshd: `sudo systemctl restart sshd`