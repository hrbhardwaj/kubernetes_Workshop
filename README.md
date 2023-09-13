# kubernetes_Workshop

This README provides a brief explanation of common Kubernetes objects and their usage.

## Pods

- **Definition**: The smallest deployable unit in Kubernetes. A Pod can contain one or more containers that share the same network and storage.
- **Use**: Deploying application components.
- **Example**: Web server + database container in a Pod.

## Services

- **Definition**: Defines a set of Pods and a policy to access them. Acts as a load balancer.
- **Use**: Exposing applications within or outside the cluster.
- **Example**: Load balancing web traffic to multiple web server Pods.

## Deployments

- **Definition**: Manages a set of identical Pods, ensuring they run and can be scaled up/down.
- **Use**: Ensuring application availability and easy updates.
- **Example**: Deploying a new version of an app while maintaining availability.

## ConfigMaps

- **Definition**: Store configuration data in key-value pairs, decoupled from Pods.
- **Use**: Separating configuration from application code.
- **Example**: Storing environment variables, config files, etc.

## Secrets

- **Definition**: Securely store sensitive information like passwords, tokens, or keys.
- **Use**: Protecting sensitive data from exposure.
- **Example**: Database passwords, API tokens.

## Persistent Volumes (PVs) & Persistent Volume Claims (PVCs)

- **Definition**: PVs represent physical storage, while PVCs are requests for storage.
- **Use**: Providing and consuming persistent storage for Pods.
- **Example**: Mounting a shared storage volume to multiple Pods.

## StatefulSets

- **Definition**: Manages stateful applications, ensuring consistent network identities.
- **Use**: Deploying databases, messaging systems, etc.
- **Example**: Running multiple database replicas with stable network identities.

## Ingress

- **Definition**: Manages external access to services within the cluster.
- **Use**: Configuring HTTP(S) routing rules for services.
- **Example**: Routing traffic to different services based on URLs.

## Jobs

- **Definition**: Runs a task to completion or until it fails.
- **Use**: Running batch jobs or one-time tasks.
- **Example**: Running data processing tasks.

## CronJobs

- **Definition**: Schedule Jobs to run periodically, similar to cron in Unix.
- **Use**: Automating recurring tasks.
- **Example**: Running backups, cleanup tasks.

## Namespace

- **Definition**: Provides a way to divide cluster resources into isolated virtual clusters.
- **Use**: Multi-tenancy, resource isolation.
- **Example**: Creating separate namespaces for development, production.

## Resources

- **Definition**: Requests and limits on CPU and memory for Pods.
- **Use**: Managing resource allocation.
- **Example**: Ensuring fair resource distribution among Pods.

## Annotations & Labels

- **Definition**: Key-value pairs used for metadata and filtering.
- **Use**: Adding information or grouping objects.
- **Example**: Marking Pods for monitoring or applying policies.

## Conclusion

This README offers a concise overview of common Kubernetes objects and their purposes. Refer to official Kubernetes documentation and specific object documentation for detailed usage and configurations.

