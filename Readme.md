# Helm Charts and Ingress Configuration

This repository contains Helm charts for two applications and an Ingress configuration.

## Project Structure

```
.
├── app-weather/          # Helm chart for weather application
├── nginx-solit/          # Helm chart for Nginx Solit application
├── ingress.yaml          # Ingress configuration
└── README.md             # This file
```

## Applications

1. **Weather Application**: Located in the `app-weather/` directory.
2. **Nginx Solit**: Located in the `nginx-solit/` directory.

Both applications are configured using Helm charts, which include templates for deployments, services, ingress, and other Kubernetes resources.

## Ingress Configuration

The `ingress.yaml` file in the root directory contains the Ingress configuration for routing traffic to both applications.

## Usage

1. Install Helm if you haven't already:
   ```
   curl https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3 | bash
   ```

2. Deploy the applications:
   ```
   helm install weather ./app-weather
   helm install nginx ./nginx-solit
   ```

3. Apply the Ingress configuration:
   ```
   kubectl apply -f ingress.yaml
   ```

## Customization

To customize the deployments, modify the `values.yaml` files in each application's directory.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

[Specify your license here]
```

Would you like me to explain or elaborate on any part of this README?