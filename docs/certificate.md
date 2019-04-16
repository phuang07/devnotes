# Certication

## Let's encrypt
```
## Check expiration date
openssl x509 -noout -dates -in /etc/letsencrypt/live/[xxxx]/cert.pem


## Dry run renew
sudo certbot --dry-run renew


## Renew
sudo certbot renew

```
