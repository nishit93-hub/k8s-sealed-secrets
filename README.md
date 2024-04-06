# k8s-sealed-secrets

    kubectl apply -f controller-2.15.2.yaml

# Download KubeSeal

    curl -L -o /tmp/kubeseal.tar.gz \
    https://github.com/bitnami-labs/sealed-secrets/releases/download/v0.19.1/kubeseal-0.19.1-linux-amd64.tar.gz
    tar -xzf /tmp/kubeseal.tar.gz -C /tmp/
    chmod +x /tmp/kubeseal
    mv /tmp/kubeseal /usr/local/bin/

**Create a sealed secret using a YAML file:**

**Example**

    kubeseal -f secret.yaml -o yaml > sealed-secret.yaml
