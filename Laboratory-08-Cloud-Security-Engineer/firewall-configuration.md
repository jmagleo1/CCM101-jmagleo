# Firewall Configuration

## Allow SSH

```bash
sudo ufw allow ssh
```

This command allows SSH (Port 22) so administrators can remotely access the server.

## Set the Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

These commands block all incoming traffic by default while allowing outgoing connections from the server.

## Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

This command allows users to access the web application running on port 8080.

## Why SSH Should Be Allowed First

If I run `sudo ufw enable` before `sudo ufw allow ssh`, the firewall may block SSH connections and I could lose remote access to the server.
