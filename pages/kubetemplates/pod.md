# Pod

    apiVersion: v1
    kind: Pod
    metadata:
      name: nginx
      labels:
        environment: production
        app: nginx
    spec:
      containers:
      - name: nginx
        image: nginx:1.14.2
        command: ["sleep"]
        args: ["infinity"]
        ports:
        - containerPort: 80
