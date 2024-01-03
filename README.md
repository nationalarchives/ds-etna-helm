# Helm Charts

```sh
# Set a secret key
export SECRET_KEY=mysecretkey123

# Install the Helm chart with develop values
helm install frontend frontend/ --namespace etna --values frontend/values.yaml --values frontend/values-dev.yaml --set env.SECRET_KEY=$SECRET_KEY

# Once done, uninstall the Helm chart
helm uninstall --namespace etna frontend
```