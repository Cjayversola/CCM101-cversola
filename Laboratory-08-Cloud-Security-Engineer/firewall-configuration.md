# Firewall Configuration

## 1. Allow SSH Access

Command:

```bash
sudo ufw allow ssh
```

This command allows SSH connections so administrators can remotely manage the server.

## 2. Set Default Firewall Policies

Commands:

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

These commands block all incoming traffic by default while allowing outgoing traffic.

## 3. Enable UFW Firewall

Command:

```bash
sudo ufw enable
```

This command activates the firewall and applies the configured rules.

## 4. Allow Port 8080

Command:

```bash
sudo ufw allow 8080/tcp
```

This command allows TCP traffic through port 8080 so users can access the web application.

## 5. Verify Firewall Rules

Commands:

```bash
sudo ufw status verbose
sudo ufw status numbered
```

These commands display the firewall status and the configured firewall rules.

## Security Reminder

If `sudo ufw enable` is executed before `sudo ufw allow ssh`, incoming SSH connections may be blocked, which could prevent administrators from remotely accessing the server.
