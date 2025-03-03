# rag-content

## Verify Image Signature

You can verify that the image stored in [quay.io/openstack-lightspeed/rag-content](quay.io/openstack-lightspeed/rag-content-openstack)
was generated by Workflow from this repository by using [cosign](https://github.com/sigstore/cosign)
utility:

```
IMAGE=quay.io/openstack-lightspeed/rag-content@sha256:<sha256sum>
cosign verify --key https://raw.githubusercontent.com/openstack-lightspeed/rag-content/refs/heads/main/.github/workflows/cosign.pub ${IMAGE}
```
