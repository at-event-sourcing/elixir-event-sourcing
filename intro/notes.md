- the command handler needs the state to validate the command, while the event handler needs the state to produce new state

- first event sourcing law: “All Events Are Immutable and Past Tense.”

- second law of event sourcing: “Applying a Failure Event Must Always Return the Previous State.”

- an aggregate is a single, uniquely identifiable entity that has state, validates commands, and emits events. An aggregate applies a function to a command to
produce events. That same aggregate also applies another function to a stream of events to produce the internal state used for validating those commands.

- The key is to anticipate your consumers.  You can design your read model so that the data required to answer any query is pregenerated,

- taking incoming information from the write model and using it to pregenerate data in anticipation of consumer queries is at the heart of event sourcing and the concept of projections.

- “All Data Required for a Projection Must Be on the Events.”