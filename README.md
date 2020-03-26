# x11-k8s-poc
A proof-of-concept for X11 apps as K8S jobs

## Usage
### Create a job (xclock)
```bash
kubectl create -f xclock-job.yml
```

### List jobs
```bash
kubectl get jobs
```

### Delete a job
Note: The display may stay on the screen a few seconds after deleting the jobs.

If the job you want to delete is `xclock-dh57z`:
```bash
kubectl delete job xclock-dh57z
```

If you want to delete all jobs (**CAUTION: this may delete jobs not related to this PoC**):
```bash
kubectl delete job --all
```
