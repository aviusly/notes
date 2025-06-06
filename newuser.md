### New User Commands

Client

`bash`
ssh-keygen -t ed25519

Follow steps, no input just `Enter`


`bash`
sudo useradd -m <newuser>
sudo usermod -aG sudo <newuser>
sudo passwd <newuser> (add password)
sudo su <newuser>
chsh <newuser> -s /bin/bash
exit
sudo su <newuser>
whoami (<newuser>)
sudo whoami (root)

`bash`
sudo su <newuser>
vi .ssh/authorized_keys
(paste id_ed25519.pub)
:wq!
