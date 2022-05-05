*********************************
Go to nginx ingress service
in annotations
1) service.beta.kubernetes.io/aws-load-balancer-protocol: http
2) service.beta.kubernetes.io/aws-load-balancer-ssl-ports: https
3) service.beta.kubernetes.io/aws-load-balancer-ssl-cert: my-cert-arn
change:
    httpPort:
      targetPort: http
    httpsPort:
      targetPort: http
