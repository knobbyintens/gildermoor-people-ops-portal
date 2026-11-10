# Dispatch Platform Release Ledger

This ledger is the authoritative record of releases rolled out to the `dispatch`
cluster. Add one row per container in a release once the rollout is verified.

| Release | Chart version | Component | Container image | Values reference |
| --- | --- | --- | --- | --- |

Column notes:

- `Release` - Helm release name.
- `Chart version` - exact chart version running in the cluster.
- `Component` - container name from the chart's pod template.
- `Container image` - the fully resolved image reference observed on the running workload.
- `Values reference` - `<chart values path>#L<line>`, where the line is the `image.repository` declaration for that component in `charts/dispatch-core/values.yaml`.

Rows are appended directly below the table header.
