# Notes

```
AWS_DEFAULT_PROFILE=this_one s3cmd sync --ssl --acl-public -M -r public/ s3://my_domain.io/ --delete-removed

aws s3 sync public/ s3://my_domain.io --delete --acl public-read --region=us-west-2 --profile this_one
```

Both upload ```public/css/nix.css``` after building the site w/ ```hugo -t nix -D -b "http://my_domain.io"```
except for some reason, the commands on travis delete and don't upload public/css/nix.css


### TODO:
* Override layouts directory and checkout latest theme every time.
