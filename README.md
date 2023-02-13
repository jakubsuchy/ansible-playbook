# ansible-playbook

# proxy.yaml
Installs and configures HAProxy using a Jinja template for all webservers

# httpd.yaml
Installs and configures Apache2 on webservers and adds a default index file that outputs server IP

# security.yaml
Adds non admin user
Adds SSH key
Configures sudo for the new user
Changes sshd config to disallow password auth

# iptables.yaml
Allows ports 22,80,2222
Forwards port 2222 to 22 - this is only for fun, no real security
Drops everything else
Save iptables rules and install post reboot script so rules survive restart
