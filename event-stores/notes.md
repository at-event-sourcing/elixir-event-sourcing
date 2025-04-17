
three key types of persistent data

- Aggregate state (snapshots) Aggregate state, as you’ve seen, is a snapshot of data produced by
applying a function to an event stream

- Projections (materialized views, read model)  While they’re also produced by applying functions
to an event stream, their shape can vary greatly across different applications
and domains. 

- Event Log (write model) only source of truth within an event-sourced system

