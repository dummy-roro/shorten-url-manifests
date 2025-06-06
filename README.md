# 🔗 URL Shortener - Golang App (Kubernetes Deployment)

A lightweight URL shortener service built with Golang, deployable to any Kubernetes cluster.

## 📝 Project Structure

This repo contains:

- `deployment.yaml`: Kubernetes manifest file to deploy the app.
- `README.md`: Documentation for deploying the app.

## 🚀 Features

- Shortens long URLs into easy-to-share links
- Built in Go for performance and low memory usage
- Kubernetes-native deployment with optional Ingress support

## 📦 Prerequisites

- Kubernetes Cluster (local or cloud-based)
- `kubectl` CLI configured
- (Optional) Ingress Controller (e.g., NGINX)

## 📁 Files

```bash
.
├── manifests           # K8s manifest files
└── README.md           # You're reading this!
```

## ⚙️ How to Deploy

### 1. Clone the Repository

```bash
git clone https://github.com/dummy-roro/shorten-url-manifests.git
cd shorten-url-manifests
```

### 2. Apply Kubernetes Manifest

```bash
kubectl apply -f deployment.yaml
```

### 3. Verify Deployment

```bash
kubectl get pods
kubectl get svc
```

Access your service via `NodePort` or `Ingress` depending on your setup.

## ✏️ Customization

Update the `deployment.yaml` file to customize:

- Docker image
- Environment variables (e.g., database URL, secret keys)
- Resource limits
- Ingress hostname (if using Ingress)

## 📤 Cleanup

To remove the deployment:

```bash
kubectl delete -f deployment.yaml
```

## 📄 License

This project is licensed under the MIT License.
