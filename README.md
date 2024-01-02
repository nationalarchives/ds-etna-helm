# Helm Charts

```sh
# Set a secret key
export SECRET_KEY=mysecretkey123

# Install the Helm chart with develop values
helm install etna-frontend frontend/ --values frontend/values.yaml --values frontend/values-develop.yaml --set env.SECRET_KEY=$SECRET_KEY

# Once done, uninstall the Helm chart
helm uninstall etna-frontend
```