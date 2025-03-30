# HOW TO USE THE SMEE PROXY

## Set up a Smee Online Webhook Proxy
Go to https://smee.io/ and start a new channel

Copy the url provided

## Use this express server to proxy to a local API
The Smee Webhook you have created will receive events. We will now use the Smee package to use the webhook and forward events to a local API

To run the Smee proxy, simply run:

```npx smee-client --url <smee URL> --path <local api path> --port <local api port>```

For example, assume the following:
- We are using Smee URL https://smee.io/AcIAVdnN2sdDsS3
- We are using a locally hosted API on port 3002 and want to forward on the path /api/v2/xyz

Then our CLI command will be:
```npx smee-client --url https://smee.io/AcIAVdnN2sdDsS3 --path /api/v2/xyz --port 3002```

test8