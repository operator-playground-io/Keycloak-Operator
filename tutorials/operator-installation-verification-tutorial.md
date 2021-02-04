---
title: Keycloak Operator Installation Verification Tutorial
description: This tutorial explains how to verify that the Keycloak Operator installed properly in the namespace
---

### Check the Keycloak Operator

After installation, verify that operator is installed successfully by executing the below command.

```execute
kubectl get csv -n my-keycloak-operator
```

You should see a similar output as below.

```output
NAME                        DISPLAY             VERSION   REPLACES                    PHASE
keycloak-operator.v12.0.1   Keycloak Operator   12.0.1    keycloak-operator.v11.0.0   Succeeded
```

**Please wait till `PHASE` status will be `Succeeded` and then proceed further.**

After the installation is successful , you can check your operator's pod by executing the below command.

```execute
kubectl get pods -n my-keycloak-operator
```

You should see a pod starting with 'Keycloak-operator' with Ready value '1/1' and Status 'Running' like the output as below.

```output
NAME                                 READY   STATUS    RESTARTS   AGE
keycloak-operator-668cc5dc75-krw9m   1/1     Running   0          92s
```