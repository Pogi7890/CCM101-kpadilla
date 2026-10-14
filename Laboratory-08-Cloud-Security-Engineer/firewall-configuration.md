# UFW Security Configuration

## SSH Access Rule

```bash
sudo ufw allow ssh
```

SSH access is permitted first to reduce the risk of losing remote administration access.

## Default Policies

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The server rejects unsolicited incoming connections while allowing outbound traffic.

## Activate UFW

```bash
sudo ufw enable
```

The firewall starts enforcing the configured policies.

## Permit the Required Web Port

```bash
sudo ufw allow 8080/tcp
```

Only the required web application port is explicitly opened for TCP traffic.

## Inspect and Test

```bash
sudo ufw status verbose
sudo ufw status numbered
curl http://localhost:8080
```

The status commands show the active policies and numbered rules. The curl command checks whether the local web application responds.

## Why SSH Must Be Allowed First

Enabling UFW before permitting SSH can block remote administrative connections, potentially locking the administrator out of the server.
