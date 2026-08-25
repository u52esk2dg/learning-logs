# Cilium Hubble Notes

- Date: 2026-08-25
- Topic: Hubble observability for cluster network policies

## Useful commands

```bash
cilium hubble enable
cilium hubble port-forward&
hubble status
hubble observe --from-pod default/nginx
```

## Observations

- Hubble flows show dropped packets by policy before egress logs.
- `--verdict` filter helps debug policy denials.
- UI is easier for spotting repeated drops.
