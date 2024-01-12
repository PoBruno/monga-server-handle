[![GitHub Repo Views](https://img.shields.io/badge/dynamic/json?color=blue&label=Repo%20Views&query=total_count&url=https%3A%2F%2Fapi.github.com%2Frepos%2FMongaDev%2Fmoga-server-handle)](https://github.com/MongaDev/moga-server-handle)
[![Last GitHub Action](https://img.shields.io/github/workflow/status/MongaDev/moga-server-handle/Start%20Game%20Server?label=Last%20Action&logo=github)](https://github.com/MongaDev/moga-server-handle/actions)

# Moga Server Handle

Repository for managing Docker images and GitHub Actions related to game servers. This repository includes scripts for starting, stopping, and backing up game servers using Docker Compose and GitHub Actions.

## Supported Games:
- Minecraft
- Project-Zomboid
- VRising
- Counter-Strike 2
- Necesse

## Upcoming Games:
- Valheim
- Terraria
- Battlefield 1942
- Rust
- The Forest

Feel free to contribute and add support for your favorite games!

## Usage:
1. Clone this repository.
2. Configure secrets for your game servers in GitHub.
3. Use the provided GitHub Actions to start, stop, and backup your game servers.

## Scripts and Commands:

### Starting a Game Server (Example: Project-Zomboid):
```bash
# Clone the repository
git clone https://github.com/MongaDev/moga-server-handle.git

# Navigate to the game server directory
cd moga-server-handle/project-zomboid

# Copy the Docker Compose configuration
cp docker-compose.yml docker-compose.yml.bak

# Set environment variables in .env file (example variables)
echo "ADMINPASSWORD=your_admin_password" >> .env
echo "DEBUG=true" >> .env
# ... (add other variables)

# Start the game server
docker-compose up -d
Stopping a Game Server:
bash
Copy code
# Navigate to the game server directory
cd moga-server-handle/project-zomboid

# Stop the game server:
docker-compose down
```

Backing Up Game Saves:
Backups are automated through GitHub Actions on each push event.

Contributions:
Contributions and feedback are welcome. If you encounter issues or want to add support for additional games, create a pull request or open an issue.

This repository is part of the MongaDev organization's tech and development experiments.
