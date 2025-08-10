to have NVIDIA GPU acceleration:


sudo apt-get update
sudo apt-get install -y nvidia-driver-535 nvidia-container-toolkit
sudo nvidia-ctk runtime configure --runtime=docker
sudo systemctl restart docker


# To Run:
```
docker compose exec -it ollama bash
ollama run deepseek-r1:8b --verbose
docker exec -it ollama ollama run deepseek-r1:8b --verbose


# Models:

deepseek-r1:latest 5.2GB 128K Text
deepseek-r1:1.5b 1.1GB 128K Text
deepseek-r1:7b 4.7GB 128K Text
deepseek-r1:8b latest 5.2GB 128K Text
deepseek-r1:14b 9.0GB 128K Text
deepseek-r1:32b 20GB 128K Text
deepseek-r1:70b 43GB 128K Text
deepseek-r1:671b 404GB 160K Text

```
