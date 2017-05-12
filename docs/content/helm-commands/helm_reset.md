+++
title = "helm reset"
weight = "34"

tags = ["commands"]
section = "helm-commands"
categories = ["helm-commands"]
type = "page"

slug = "helm-reset"

[menu.main]
  url = "helm-reset"
  parent = "helm-commands"

+++

## helm reset

uninstalls Tiller from a cluster

### Synopsis



This command uninstalls Tiller (the helm server side component) from your
Kubernetes Cluster and optionally deletes local configuration in
$HELM_HOME (default ~/.helm/)


```
helm reset
```

### Options

```
  -f, --force                forces Tiller uninstall even if there are releases installed
      --remove-helm-home     if set deletes $HELM_HOME
      --tls                  enable TLS for request
      --tls-ca-cert string   path to TLS CA certificate file (default "$HELM_HOME/ca.pem")
      --tls-cert string      path to TLS certificate file (default "$HELM_HOME/cert.pem")
      --tls-key string       path to TLS key file (default "$HELM_HOME/key.pem")
      --tls-verify           enable TLS for request and verify remote
```

### Options inherited from parent commands

```
      --debug                     enable verbose output
      --home string               location of your Helm config. Overrides $HELM_HOME (default "~/.helm")
      --host string               address of tiller. Overrides $HELM_HOST
      --kube-context string       name of the kubeconfig context to use
      --tiller-namespace string   namespace of tiller (default "kube-system")
```

### SEE ALSO
* [helm](#helm)	 - The Helm package manager for Kubernetes.