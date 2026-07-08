
## ONY KASIDIKA Jordan

## Capture d'écran

> ![kubet get all](file:///C:/Users/Hp/Desktop/TP%20-%20ADM%20RES/kubet%20get%20all.jpg)

```bash
kubectl get all
```

Cette capture doit afficher les **Pods**, **Services** et **ReplicaSets** déployés dans le cluster Kubernetes.

---

## Intérêt d'utiliser un objet Service

Un objet **Service** fournit un point d'accès stable aux applications, même si les Pods sont recréés ou changent d'adresse IP. Il répartit automatiquement le trafic entre les différents Pods disponibles (load balancing) et garantit une communication fiable entre les composants de l'application. Cela évite de devoir utiliser directement les adresses IP des Pods, qui sont temporaires.

---

## Mise à l'échelle (Scaling)

Pour augmenter le nombre de réplicas de **3 à 10**, utilisez la commande suivante :

```bash
kubectl scale deployment <nom_du_deployment> --replicas=10
```
