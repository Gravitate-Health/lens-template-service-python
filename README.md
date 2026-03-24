# lens-template-service-python
An example of an external service implementing a lense using Python

## Deployment

### Deploy via Helm (OCI)

```bash
# Login to registry (if private)
helm registry login ghcr.io

# Deploy directly from the registry
helm install my-release oci://ghcr.io/<your-org>/charts/<chart-name> --version <version>
```

### Local Development

```bash
helm lint charts/lens-template-service-python
helm template my-release charts/lens-template-service-python
```
