# 🃏 Yu-Gi-Oh! DevOps Deck

Questo progetto è un'applicazione web "Evocata Specialmente" su un cluster Kubernetes locale. 

## 🛠️ Tech Stack
* **Docker**: Containerizzazione dell'app con Nginx.
* **Kubernetes (k3d)**: Orchestrazione e gestione dei Pod.
* **Infrastructure as Code**: Gestione del cluster tramite file YAML.
* **Cloud Native**: Concetti applicati dalla certificazione AWS Cloud Practitioner.

## 🚀 Come lanciarlo
1. Build dell'immagine: \`docker build -t mio-sito-k8s:v1 .\`
2. Import nel cluster: \`k3d image import mio-sito-k8s:v1 -c cluster-portfolio\`
3. Deploy: \`kubectl apply -f app.yaml\`
4. Accesso: \`kubectl port-forward service/sito-service 8081:80\`
