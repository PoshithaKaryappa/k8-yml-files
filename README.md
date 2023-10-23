#simple kube pods
apiVersion: v1
kind: Pod
metadata:
    name: hello-pod
    labels:
      app: web
spec:
    containers:
       - name: web-ctr
       image: nigelpoulton/getting-started-k8s:0.0
       ports:
          - containerPort: 8080
            protocol: TCP
