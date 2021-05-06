# hwf

```
kubebuilder init --domain x-helm.dev --skip-go-version-check
kubebuilder edit --multigroup=true

kubebuilder create api --group module --version v1alpha1 --kind Workflow
```

```
make install
make run
```

```
make docker-build docker-push IMG=appscodeci/hwf:v0.1.0
make deploy IMG=appscodeci/hwf:v0.1.0
```

```
$ kubectl ns hwf-system
$ kubectl get pods
NAME                                      READY   STATUS    RESTARTS   AGE
hwf-controller-manager-5956dd7759-n6dbt   1/2     Running   0          21s
```
