# Replication controller
# step to create
1) Create one ubuntu instance
2) Switch to root user by the command sudo-i
3)install docker by the belown cmd
sudo apt install curl wget apt-transport-https -y
sudo curl -fsSL https://get.docker.com -o get-docker.sh
chmod 777 get-docker.sh
sh get-docker.sh
# Installation of minikube by the commands
sudo curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo mv minikube-linux-amd64 /usr/local/bin/minikube
sudo chmod +x /usr/local/bin/minikube
sudo minikube version
# . Installation of kubectl by the commands
sudo curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl
sudo curl -LO "https://dl.k8s.io/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl.sha256
sudo echo "$(cat kubectl.sha256) kubectl" | sha256sum --check
sudo install -o root -g root -m 0755 kubectl/usr/local/bin/kubect
sudo install -o root -g root -m 0755 kubectl/usr/local/bin/kubectl
sudo kubectl version --client --output=yaml
sudo minikube start --driver=docker --force
# Create the pod belown commands
kubectl run pod-name --image=image-name
create yam file vi prashanth.yml
![Screenshot 2024-11-18 194723](https://github.com/user-attachments/assets/76a2d202-ff9e-4333-828d-88c0dda2b1ed)
 kubectl create -f prashanth.yml - by this command if pod is created then the work is done
 ![Screenshot 2024-11-18 202336](https://github.com/user-attachments/assets/1d6e5627-2b5c-46cd-b1b5-298dddf83ac3)

