## ArgoCD ##


Step 1: Create kubernetes deployment with above cluster image

```
 kubectl apply -f deployment.yaml

 kubectl apply -f nginx-service.yaml 

```


Step 2: Add ingress service 
```
 kubectl apply -f ingress.yaml

```
## Test deployment ##

Test the challenge using below command:

```
minikube service blog-argocd --url

curl {url}

Output:
<!doctype html>
<html>
  <head>
    <title>Hello nginx</title>
    <meta charset="utf-8" />
  </head>
  <body>
    <h1>
        Hello CGI! 
    </h1>
  </body>
</html>
```
### TODO ###
Step 5: CI/CD pipeline (optional)

