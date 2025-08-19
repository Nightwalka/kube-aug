

```markdown
# Kubernetes Practice Manifests

This repo contains example Kubernetes manifests for practice and learning.  
Each YAML file demonstrates different Kubernetes objects and deployment strategies.

## 📂 Project Structure

```

.
├── deployments
│   ├── deployment-2.yaml   # Alternative Deployment example
│   └── deployment.yaml     # Basic Deployment definition
├── ngix.yaml               # Nginx Deployment/Service example
├── redic.yaml              # Redis Deployment/Service example
└── rolling.yaml            # Rolling update strategy example

````

## 🚀 Usage

Apply any manifest to your cluster using:

```bash
kubectl apply -f <filename>.yaml
````

For example:

```bash
kubectl apply -f ngix.yaml
```

To check the created resources:

```bash
kubectl get all
```

## 🔄 Updating a Deployment

To trigger a rolling restart:

```bash
kubectl rollout restart deployment <deployment-name>
```

To check rollout status:

```bash
kubectl rollout status deployment <deployment-name>
```

## 🧹 Cleanup

Remove all resources created:

```bash
kubectl delete -f <filename>.yaml
```

Or delete everything in this directory:

```bash
kubectl delete -f .
```

---

📝 **Note:** These manifests are for learning purposes only. They are not production-ready.

```

---

Want me to also add **step-by-step practice tasks** (e.g., “Deploy Redis, scale it, then apply rolling.yaml for updates”) so it’s like a mini lab guide?
```
