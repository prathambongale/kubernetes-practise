# kubernetes-practise
This is repository has all kubernetes practise files 

## kubernetes definition file
- Top level field:

    >apiVersion: 
    
    >kind:

    >metadata:

    >spec:

    ---    
    Possible values for apiVersion and kind
        
    | Kind |Version |
    |-----------|:-----------:| 
    | [Pod](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/pod-v1/) | `v1` |
    | [PodTemplate](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/pod-template-v1/) | `v1` |
    | [ReplicationController](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/replication-controller-v1/) | `v1` |
    | [ReplicaSet](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/replica-set-v1/) | `apps/v1` |
    | [Deployment](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/deployment-v1/) | `apps/v1` |
    | [StatefulSet](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/stateful-set-v1/) | `apps/v1` |
    | [ControllerRevision](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/controller-revision-v1/) | `apps/v1` |
    | [DaemonSet](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/daemon-set-v1/) | `apps/v1` |
    | [Job](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/job-v1/) | `batch/v1` |
    | [CronJob](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/cron-job-v1/) | `batch/v1` |
    | [HorizontalPodAutoscaler](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/horizontal-pod-autoscaler-v1/) | `autoscaling/v1` |
    | [HorizontalPodAutoscaler](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/horizontal-pod-autoscaler-v2beta2/) | `autoscaling/v2beta2` |
    | [PriorityClass](https://kubernetes.io/docs/reference/kubernetes-api/workload-resources/priority-class-v1/) | `scheduling.k8s.io/v1` |
    | [Service](https://kubernetes.io/docs/reference/kubernetes-api/service-resources/service-v1/) | `v1` |
    | [Endpoints](https://kubernetes.io/docs/reference/kubernetes-api/service-resources/endpoints-v1/) | `v1` |
    | [EndpointSlice](https://kubernetes.io/docs/reference/kubernetes-api/service-resources/endpoint-slice-v1/) | `discovery.k8s.io/v1` |
    | [Ingress](https://kubernetes.io/docs/reference/kubernetes-api/service-resources/ingress-v1/) | `networking.k8s.io/v1` |
    | [IngressClass](https://kubernetes.io/docs/reference/kubernetes-api/service-resources/ingress-class-v1/) | `networking.k8s.io/v1` |
    | [ConfigMap](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/config-map-v1/) | `v1` |
    | [Secret](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/secret-v1/) | `v1` |
    | [PersistentVolumeClaim](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-claim-v1/) | `v1` |
    | [PersistentVolume](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-v1/) | `v1` |
    | [StorageClass](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/storage-class-v1/) | `storage.k8s.io/v1` |
    | [VolumeAttachment](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/volume-attachment-v1/) | `storage.k8s.io/v1` |
    | [CSIDriver](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/csi-driver-v1/) | `storage.k8s.io/v1` |
    | [CSINode](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/csi-node-v1/) | `storage.k8s.io/v1` |
    | [CSIStorageCapacity](https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/csi-storage-capacity-v1beta1/) | `storage.k8s.io/v1beta1` |
    | [ServiceAccount](https://kubernetes.io/docs/reference/kubernetes-api/authentication-resources/service-account-v1/) | `v1` |
    | [TokenRequest](https://kubernetes.io/docs/reference/kubernetes-api/authentication-resources/token-request-v1/) | `authentication.k8s.io/v1` |
    | [TokenReview](https://kubernetes.io/docs/reference/kubernetes-api/authentication-resources/token-review-v1/) | `authentication.k8s.io/v1` |
    | [CertificateSigningRequest](https://kubernetes.io/docs/reference/kubernetes-api/authentication-resources/certificate-signing-request-v1/) | `certificates.k8s.io/v1` |
    | [LocalSubjectAccessReview](https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/local-subject-access-review-v1/) | `authorization.k8s.io/v1` |
    | [SelfSubjectAccessReview](https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/self-subject-access-review-v1/) | `authorization.k8s.io/v1` |
    | [SelfSubjectRulesReview](https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/self-subject-rules-review-v1/) | `authorization.k8s.io/v1` |
    | [SubjectAccessReview](https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/subject-access-review-v1/) | `authorization.k8s.io/v1` |
    | [ClusterRole](https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/cluster-role-v1/) | `rbac.authorization.k8s.io/v1` |
    | [ClusterRoleBinding](https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/cluster-role-binding-v1/) | `rbac.authorization.k8s.io/v1` |
    | [Role](https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/role-v1/) | `rbac.authorization.k8s.io/v1` |
    | [RoleBinding](https://kubernetes.io/docs/reference/kubernetes-api/authorization-resources/role-binding-v1/) | `rbac.authorization.k8s.io/v1` |
    | [LimitRange](https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/limit-range-v1/) | `v1` |
    | [ResourceQuota](https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/resource-quota-v1/) | `v1` |
    | [NetworkPolicy](https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/network-policy-v1/) | `networking.k8s.io/v1` |
    | [PodDisruptionBudget](https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/pod-disruption-budget-v1/) | `policy/v1` |
    | [PodSecurityPolicy](https://kubernetes.io/docs/reference/kubernetes-api/policy-resources/pod-security-policy-v1beta1/) | `policy/v1beta1` |
    | [CustomResourceDefinition](https://kubernetes.io/docs/reference/kubernetes-api/extend-resources/custom-resource-definition-v1/) | `apiextensions.k8s.io/v1` |
    | [MutatingWebhookConfiguration](https://kubernetes.io/docs/reference/kubernetes-api/extend-resources/mutating-webhook-configuration-v1/) | `admissionregistration.k8s.io/v1` |
    | [ValidatingWebhookConfiguration](https://kubernetes.io/docs/reference/kubernetes-api/extend-resources/validating-webhook-configuration-v1/) | `admissionregistration.k8s.io/v1` |
    | [Node](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/node-v1/) | `v1` |
    | [Namespace](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/namespace-v1/) | `v1` |
    | [Event](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/event-v1/) | `events.k8s.io/v1` |
    | [APIService](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/api-service-v1/) | `apiregistration.k8s.io/v1` |
    | [Lease](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/lease-v1/) | `coordination.k8s.io/v1` |
    | [RuntimeClass](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/runtime-class-v1/) | `node.k8s.io/v1` |
    | [FlowSchema](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/flow-schema-v1beta1/) | `flowcontrol.apiserver.k8s.io/v1beta1` |
    | [PriorityLevelConfiguration](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/priority-level-configuration-v1beta1/) | `flowcontrol.apiserver.k8s.io/v1beta1` |
    | [Binding](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/binding-v1/) | `v1` |
    | [ComponentStatus](https://kubernetes.io/docs/reference/kubernetes-api/cluster-resources/component-status-v1/) | `v1` |
    ---

