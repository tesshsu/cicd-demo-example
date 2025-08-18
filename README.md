# CICD Demo Example

*This repository demonstrates a basic CI/CD setup for Kubernetes deployment using GitHub Actions and Kustomize.*

## Structure

- `.github/workflow/deploy.yml` — CI/CD pipeline example using GitHub Actions.
- `k8s/base/deployment.yaml` — Standard Kubernetes Deployment manifest (base).
- `k8s/overlays/production/kustomization.yaml` — Example overlay to patch deployment (Kustomize canary rollout etc).
- `k8s/prometheus-alert.yaml` — Example Prometheus alert rule for error monitoring.
- `index.html` — Example application file.

> **Note:** All registry URLs and deployment names use `example.com` and demo names for safety—this repo is for educational/demo purposes only.

---

## Canary Deployments and Alerting

The repo demonstrates:
- Safe canary deployments using Kustomize overlays with a patched replica count and canary label.
- Example Prometheus alerting to notify if error rates spike after deployment.

---

## Learn More

For background, explanations, and step-by-step context, please check my blog post:

👉 [https://tesshsu.github.io/blogs/blog-19.html](https://tesshsu.github.io/blogs/blog-19.html)

This repository is an example only. For more detail, see the linked blog.

---
