# dd-ddi-lab

Authorized self-owned lab for a private Datadog HackerOne engagement.

- Own kind cluster (Kubernetes 1.32, one node) and own Datadog US1 organization.
- Tests whether the `DatadogInstrumentation` CRD (provider `instrumentation-checks`, default Helm chart 3.269.1, agent/Cluster Agent 7.85.4) delivers `spec.config.checks` to the node agent, and whether a `jmx` instance's `java_bin_path`/`java_options` executes a command as the agent's uid while `integration_ignore_untrusted_file_params: true`.
- Only canary marker files under `/tmp`; no third-party infrastructure, no customer data, no destructive actions.
