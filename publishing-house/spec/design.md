# Installing Red Hat build of Keycloak Operator on OpenShift

## Overview

This lab covers the installation of the Red Hat build of Keycloak (RHBK) operator on an OpenShift 4.22 cluster. RHBK is the enterprise-supported identity and access management solution built on the Keycloak project. Participants will navigate to OperatorHub, install the RHBK operator, and confirm it is running and ready to manage Keycloak instances.

## Target Audience

- **Role:** Platform engineers
- **Experience level:** Advanced
- **What they already know:** OpenShift cluster administration, OperatorHub, operator lifecycle management (OLM), cluster-admin access
- **What they don't know:** How to install and verify the Red Hat build of Keycloak operator specifically

## Prerequisites

- Access to an OpenShift 4.22 cluster with cluster-admin privileges
- Familiarity with OperatorHub and OpenShift operator lifecycle management
- Can the lab validate these automatically? No — trust-based (classic Showroom, no automated prerequisite check)

## Learning Objectives

1. Install the Red Hat build of Keycloak operator on an OpenShift cluster using OperatorHub
2. Verify the operator deployment is healthy and ready to manage Keycloak instances

## Content Type

Lab (hands-on)

## Products & Technologies

- Red Hat build of Keycloak
- Red Hat OpenShift Container Platform 4.22

## Module Map

| Module | Title | Duration |
|--------|-------|----------|
| 1 | Installing the Red Hat build of Keycloak Operator | 15 min |
| — | **Total hands-on** | **15 min** |
| — | Intro / presentation | ~5 min |
| — | **Total lab** | **~20 min** |

## Difficulty Level

Advanced

## Environment

**Learner view:** A running OpenShift 4.22 cluster is provisioned and accessible. Participants log in to the OpenShift web console with cluster-admin credentials. OperatorHub is available and connected to the Red Hat operator catalog.

**Automation needed:** No — a running OpenShift 4.22 cluster with OperatorHub connected to the Red Hat catalog is pre-provisioned; no per-user resource provisioning required beyond cluster access.

## Infrastructure Requirements

- **Cloud provider:** CNV
- **Cluster type:** SNO (Single Node OpenShift)
- **OCP version:** 4.22
- **Topology:** Per-student
- **Sizing:** 1 control plane node (32 vCPU, 128 GB RAM) — SNO, no separate workers
- **Automation approach:** OLM (Operator Lifecycle Manager) — operator installed by participant via OperatorHub
- **AI/MaaS:** None
- **External services:** registry.redhat.io, registry.access.redhat.com
- **AAP version:** N/A
- **Non-GA products:** None (all products are GA)
