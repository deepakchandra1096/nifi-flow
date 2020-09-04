# Usage
The first step to using Cloud Custodian is writing a YAML file containing the policies that you want to run. Each policy specifies the resource type that the policy will run on, a set of filters which control resources will be affected by this policy, actions which the policy with take on the matched resources, and a mode which controls which how the policy will execute.
You can validate, test, and run Cloud Custodian with the example policy with these commands:
```
# Validate the configuration (note this happens by default on run)
$ custodian validate policy.yml

# Dryrun on the policies (no actions executed) to see what resources
# match each policy.
$ custodian run --dryrun -s out policy.yml

# Run the policy
$ custodian run -s out policy.yml
```

