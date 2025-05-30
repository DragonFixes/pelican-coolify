# Pelican Coolify

This repository contains Docker Compose configurations for deploying Pelican (a game server management panel) using Coolify. There are two deployment options available:

## Deployment Options

### 1. One-Click Installation (Complete Setup)
The `one-click.yaml` file provides a complete setup that includes the MariaDB, Redis cache, Pelican panel, and Wings.

### 2. External Services Setup
The `production.yaml` file is how I personally like setting up my resources in Coolify. Basically keep the databases outside of the one-click that way I can do rolling updates without the need to take down the database, or if you have multiple services accessing the same DBs.

For simplicity sakes, I recommend using the `one-click.yaml` unless you know what you're doing.

## Environment Variables

### Required Variables
- `DB_PASSWORD`: Database password for the Pelican user
- `DB_ROOT_PASSWORD`: Root password for the database (one-click setup only)
- `PANEL_URL`: The URL where your panel will be accessible


