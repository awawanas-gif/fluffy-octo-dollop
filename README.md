# flu# Clone the project
git clone https://github.com/zhouxiaoka/autoclip.git
cd autoclip

# Docker one-click startup
./docker-start.sh

# Development environment startup
./docker-start.sh dev

# Stop services
./docker-stop.sh

# Check service status
./doc# Clone the project
git clone https://github.com/zhouxiaoka/autoclip.git
cd autoclip

# One-click startup (recommended, includes complete checks and monitoring)
./start_autoclip.sh

# Quick startup (development environment, skips detailed checks)
./quick_start.sh

# Check system status
./status_autoclip.sh

# Stop system
./stop_autoclip.shker-status.shffy-octo-dollop# 1. Create virtual environment
python3 -m venv venv
source venv/bin/activate  # Linux/macOS
# or venv\Scripts\activate  # Windows

# 2. Install Python dependencies
pip install -r requirements.txt

# 3. Install frontend dependencies
cd frontend && npm install && cd ..

# 4. Install Redis
# macOS
brew install redis
brew services start redis

# Ubuntu/Debian
sudo apt update
sudo apt install redis-server
sudo systemctl start redis-server

# CentOS/RHEL
sudo yum install redis
sudo systemctl start redis

# 5. Install FFmpeg
# macOS
brew install ffmpeg

# Ubuntu/Debian
sudo apt install ffmpeg

# CentOS/RHEL
sudo yum install ffmpeg

# 6. Configure environment variables
cp env.example .env
# Edit .env file and fill in necessary configurations
