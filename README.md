Git Ops

## Definition :

GitOps is running operations Out of Git, by Pull Requests, with the goal of continuous delivery of cloud native apps, typically to Kubernetes.
It’s considered as combination of 4 DevOps technologies and practices : IaC, Git, CI/CD, convergent platforms (api, extensible, converent).


## Use Cases :

- Continous Delivery of application configurations.
- Apply Release strategies (Rolling update, Progressive such as Blue Green and Canary).
- Infrastructure rollouts to Kubernetes (e.g. Ingress Controllers, Namespaces, RBAC Policies, Network Policies, CRDs ).
- Disaster Recovery (e.g. automatically move to a backup k8s cluster if the primary cluster is deleted for some reason ).
- Synchronise secrets (e.g. Vault <===> K8s ).
- Drift Detection ( Notify, Reconcile ) : Detect desired state changes in Git repo and apply changes to current state in K8s.
- Deploy to multiple K8s clusters (e.g. in multiple regions ).
- Securely handoff deployments to developers ( No cluster access to Devs, Multi-tenancy and separation of concerns ).
- Auto update K8s YAML files on new image push in a registry ( Auto scan a registry and update correspondent manifest files ).
