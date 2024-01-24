oc create secret generic sops-gpg --namespace=openshift-gitops \
--from-file=private-FBC7B9E2A4F9289AC0C1D4843D16CEE4A27381B4.asc \
--from-file=private-D7229043384BCC60326C6FB9D8720D957C3D3074.asc \
--from-file=private-B611A2F9F11D0FF82568805119F9B5DAEA91FF86.asc \
--dry-run=client -o yaml > secret-sops-gpg.yaml
