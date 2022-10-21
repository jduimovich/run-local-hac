# run-local-hac

# Pre-reqs

Install app-studio on your kcp-stable, the easiest way is to run the `create-user-workspace.sh appstudio` script from infra-deployments when logged into 
kcps-stable
You also need `oc`, `kubectl`, and `node.js` installed

You need to be connected to RH VPN.
You also need these in your hosts file. Note, if you are connecting to a VM or other non-local machine, you can simply point this to the machine IP
```
127.0.0.1   prod.foo.redhat.com
127.0.0.1   stage.foo.redhat.com
```

# Install
Clone this repo and run `bash install`

# Run

Make sure you are connected to kcp-stable and then run 

`bash run-hac-and-proxy`

connect to https://prod.foo.redhat.com:1337/beta/hac/app-studio 

It may take upto 60 seconds for the webpack to compile hac-dev. 
