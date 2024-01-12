
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/pobruno/monga-server-data)
[![GitHub repo size](https://img.shields.io/github/repo-size/pobruno/monga-server-data?label=monga-server-data&logo=git&logoColor=orang)](https://github.com/pobruno/monga-server-data)
![GitHub top language](https://img.shields.io/github/languages/top/pobruno/monga-server-data?logo=docker)
![GitHub language count](https://img.shields.io/github/languages/count/pobruno/monga-server-data)
![GitHub issues](https://img.shields.io/github/issues/pobruno/monga-server-data?logo=github)

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

# Backing Up Game Saves:

Backups are automated on repo [monga-server-data](https://github.com/pobruno/monga-server-data) through GitHub Actions on each push event.

# Contributions:

Contributions and feedback are welcome. If you encounter issues or want to add support for additional games, create a pull request or open an issue.

---

_This repository is part of the MongaDev organization's tech and development experiments._

