# Kubernetes Rollout Notes

- `kubectl rollout status deployment/my-app` to check progress
- Use `--timeout` to avoid hanging in CI
- `kubectl rollout undo` for quick rollback
- Always pin image digest in production
