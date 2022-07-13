
# Ubike@Taipei Nearest Search 
![image](https://user-images.githubusercontent.com/84711996/178797533-a3402e26-0cc3-44fa-b0ad-ec5f5dd9a4fc.png)
## Implement with k8s by k3d

### Create cluster
```bash
k3d cluster create mycluster --servers 1 --agents 2 -p "30000-30005:30000-30005@server:0"
```
### Apply pods
```bash
cd deploy-file
kubectl apply -f .
```
### Open browser and search the location(or with Postman)
```bash
localhost:30004/台北101
```

