# Flux vs Argo CD

Quick comparison while evaluating GitOps tools for our next setup.

| Aspect | Flux | Argo CD |
|---|---|---|
| Bootstrap | GitRepository + Kustomization | Application CRD + initial app |
| UI | No built-in UI | Full web UI |
| SSO/RBAC | Via Flux controllers | Built-in with Dex/SSO |
| Sync model | Push-based from cluster | Pull-based with automated sync |
| Multi-cluster | Manual or via Kustomization | Good with ApplicationSets |
| Learning curve | Lower, K8s native | Higher, more concepts |

Verdict: start with Flux for simpler bootstrap; revisit Argo CD if we need app-of-apps and UI.
