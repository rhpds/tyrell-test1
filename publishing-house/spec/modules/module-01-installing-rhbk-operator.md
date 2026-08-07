# Module 01 — Installing the Red Hat build of Keycloak Operator

### Brief Overview

This module walks platform engineers through installing the Red Hat build of Keycloak (RHBK) operator on an OpenShift 4.22 cluster using OperatorHub. RHBK is the enterprise-supported identity and access management solution built on the upstream Keycloak project. Participants start from the OpenShift web console, locate the RHBK operator in the Red Hat operator catalog, complete the installation wizard, and confirm the operator is healthy and ready to manage Keycloak instances.

### Audience and Time

- **Target persona:** Platform engineers with advanced OpenShift experience
- **Prerequisites for this module:** Cluster-admin access to a running OpenShift 4.22 cluster; familiarity with OperatorHub and operator lifecycle management (OLM)
- **Estimated duration:** 15 min

### Learning Objectives

- Install the Red Hat build of Keycloak operator on an OpenShift cluster using OperatorHub
- Verify the operator deployment is healthy and ready to manage Keycloak instances

### Lab Structure

| Section | Title | Duration |
|---------|-------|----------|
| 1 | Navigate to OperatorHub and locate the RHBK operator | 5 min |
| 2 | Install the RHBK operator | 5 min |
| 3 | Verify the operator is running and ready | 5 min |

### Detailed Steps

1. Log in to the OpenShift web console using cluster-admin credentials.
2. In the left navigation, expand **Operators** and click **OperatorHub**.
3. In the OperatorHub search field, enter `Red Hat build of Keycloak` and press Enter.
4. Locate the **Red Hat build of Keycloak** tile in the Red Hat operator catalog and click it.
5. Review the operator description, supported versions, and capabilities, then click **Install**.
6. On the Install Operator page, accept or adjust the default installation options (update channel, installation mode, installed namespace, and update approval strategy).
7. Click **Install** to begin the installation.
8. In the left navigation, click **Operators → Installed Operators** and select the target namespace.
9. Monitor the RHBK operator entry until its status shows **Succeeded**.
10. Confirm that the operator pod is running in the target namespace by navigating to **Workloads → Pods** and verifying pod status is **Running**.

### Key Takeaways

- OperatorHub provides a curated catalog of Red Hat-supported operators that can be installed directly from the OpenShift web console.
- The RHBK operator manages the full lifecycle of Keycloak instances on OpenShift, including installation, updates, and configuration.
- A **Succeeded** install status and a **Running** operator pod together confirm the operator is healthy and ready to manage Keycloak instances.

### Infrastructure Notes

- The OpenShift 4.22 cluster must have OperatorHub connected to the Red Hat operator catalog.
- Participants must have cluster-admin privileges to access OperatorHub and install cluster-scoped operators.
- Specific cloud provider, cluster type, topology, sizing, and automation details are TBD — to be confirmed in the infrastructure phase.
