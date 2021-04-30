# edgeworkerskv-zipcode-lookup
Demo for looking up Akamai Edgescape ZIP codes in Edge KV

## CircleCI (Optional)
CircleCI can automate the deployment to staging for this EdgeWorker on each `git commit`. The asociated configuration is in the `.circleci.yml` file.
[CircleCI Contexts](https://circleci.com/docs/2.0/contexts/]) is are used to pass on sensitive information in variables to the configuration file `.circleci.yml`. The following variables should be managed under CirecleCI Contexts for this example. 

### Account Info Variables
- $ACCOUNTKEY: Optional. Used to switch between accounts. If not needed remove all associations and the `--accountkey` flag from the commands.
- $HOSTNAME: Hostname associated to the property running EdegeWorkers. Used to create the enhanced debugging token.

### Edge KV variables
- $EDGEKV_NAMESPACE: EdgeKV namespace to build the edgekv_tokens.js
- $EDGEKV_TOKEN_NAME: EdgeKV token name to build the edgekv_tokens.js
- $EDGEKV_TOKEN_VALUE: EdgeKV token to build the edgekv_tokens.js

### Akamai API Credential Variables
- $ACCESS_TOKEN
- $HOST
- $CLIENT_SECRET
- $CLIENT_TOKEN

## More details on EdgeWorkers
- [Akamai EdgeWorkers](https://developer.akamai.com/akamai-edgeworkers-overview)
- [Akamai EdgeWorkers User Guide](https://learn.akamai.com/en-us/webhelp/edgeworkers/edgeworkers-user-guide/GUID-14077BCA-0D9F-422C-8273-2F3E37339D5B.html)
- [Akamai EdgeWorkers Examples](https://github.com/akamai/edgeworkers-examples)
- [Akamai CLI for EdgeWorkers](https://developer.akamai.com/legacy/cli/packages/edgeworkers.html)