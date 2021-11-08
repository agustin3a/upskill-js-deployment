# Upskill JS Budget App Deployment

## Local

### Database

Configure postgres user password. 

Encode password:

```
$ echo -n '{password}' | base64
```

Update secret in file **k8s/postgres.yml** with your encoded password.

Start database service/deployment:

```
$ kubectl apply -f  k8s/postgres.yml
```

## GCP

