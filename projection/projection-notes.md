- A projector is a piece of code responsible for producing read model data for consumption by one or more parties. 
The projector is AccountBalance and the projection is a piece of data containing the most up-to-date balance for a given account.

- Projectors handle events and produce views of data designed specifically with consumers in mind. In contrast,aggregates also process events to produce state, but that state is internal.

- process managers must never emit events