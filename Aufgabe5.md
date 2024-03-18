# Lösungen für Aufgabe 5

## 1. Vorteile eines Depoyments gegenüber einem Pod

Ein Pod ist die kleinste Einheit in Kubernetes, idr. nur ein Container. Ein Deployment hingegen ist eine "höhere" Einheit, welche aus mehreren Pods bestehen kann.
Weitere Vorteile

-   Rolling Updates möglich
-   Skalierung
-   Automatisches Restarten von Pods
-   Rollback auf eine frühere Version

## 2. Kubernetes Service

Ein Kubernetes Service dient dazu, (Pods, Deployments, etc.) in einem Cluster über das Netzwerk erreichbar zu machen. Dies kann entweder nur innerhalb des Clusters oder auch von außen möglich sein.

## 3. Arten von Services

-   ClusterIP: Service ist nur innerhalb des Clusters verfügbar
-   NodePort: Service ist über einen Port auf jeder Node verfügbar
-   LoadBalancer: Service ist über einen externen LoadBalancer verfügbar, welcher vom Cloud Provider bereitgestellt oder installiert werden muss (z. B. MetalLB)
-   ExternalName:
