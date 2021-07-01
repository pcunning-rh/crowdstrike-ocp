# CrowdStrike for OpenShift 4.x (semi-disconnected)

1. Build image with Dockerfile (uses UBI 8.3 for OCP 4.7/RHCOS 4.7)
2. Update `entrypoint.sh` with your CrowdStrike ID (CID).
3. Update `configmap.yaml` for parameters CID and Provisioning Token. Additional parameters can be added, visit [GHRepo](https://github.com/CrowdStrike/falcon-helm/blob/main/helm-charts/falcon-sensor/values.yaml)
4. Update `daemonset.yaml` with your image registry and image name+tag.
.... more to come