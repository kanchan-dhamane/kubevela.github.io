---
title: vela def get
---

Get definition

### Synopsis

Get definition from kubernetes cluster

```
vela def get NAME [flags]
```

### Examples

```
# Command below will get the ComponentDefinition(or other definitions if exists) of webservice in all namespaces
> vela def get webservice
# Command below will get the TraitDefinition of annotations in namespace vela-system
> vela def get annotations --type trait --namespace vela-system
```

### Options

```
  -h, --help               help for get
  -n, --namespace string   Specify which namespace the definition locates. (default "vela-system")
  -r, --revision string    Get the specified version of a definition.
      --revisions          List revisions of the specified definition.
  -t, --type string        Specify which definition type to get. If empty, all types will be searched. Valid types: policy, workload, workflow-step, component, trait
```

### Options inherited from parent commands

```
  -V, --verbosity Level   number for the log level verbosity
  -y, --yes               Assume yes for all user prompts
```

### SEE ALSO

* [vela def](vela_def)	 - Manage definitions.

#### Go Back to [CLI Commands](vela) Homepage.


###### Auto generated by [spf13/cobra script in KubeVela](https://github.com/kubevela/kubevela/tree/master/hack/docgen).