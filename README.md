# open-webui
A personal open-webui repo for docker

# Getting Started:

## Start via docker compose
cd open-webui
sudo docker compose up -d

## Start via command line
sudo docker run -p 3000:8080 --gpus all --network=host -v /home/jay/Apps/open-webui:/app/backend/data -e OLLAMA_BASE_URL=http://localhost:11434 PORT=3001 --name open-webui --restart=unless-stopped ghcr.io/open-webui/open-webui:cuda

## UI
http://localhost:3001/


# Troubleshooting:

## status check
http://localhost:3000/

# Remove
sudo docker rm -f open-webui
