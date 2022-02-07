# solace-risk-data-docs

Update swagger definitions for the Solace Risk Data API in file solace-risk_api_alpha-0.0.1-resolved.json

Remove content in S3 bucket: solace-risk-data-docs
```console
aws s3 rm s3://risk-data-docs.solace.fi --include "*" --recursive
```

Add all files from this repo to S3 bucket: solace-risk-data-docs
```console
aws s3 cp --recursive solace-risk-data-docs/ s3://risk-data-docs.solace.fi/
```