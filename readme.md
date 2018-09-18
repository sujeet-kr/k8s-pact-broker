**Pact Broker (Using Kubernetes)**

1. Create the Postgres database svc and pod that the broker is going to use -
    `kubectl -n fcpte create -f pact-postgres-deploy.yaml`
2. Create the Pact Broker svc and pod -
    `kubectl -n fcpte create -f pact-broker-deploy.yaml`
3. Get the url of the Pact UI (for Minikube)-
    `minikube -n fcpte service pact-broker --url`
