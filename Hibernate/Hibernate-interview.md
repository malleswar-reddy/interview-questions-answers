# ACID Properties for Transactions
### ACID is an acronym which stands for Atomicity, Consistency, Isolation, and Durability. This terminology is usually used in the context of databases or transactional operations.

#### Atomicity
For a transaction to be atomic, all transaction members must make the same decision. Either they all commit, or they all roll back. If atomicity is broken, what results is termed a heuristic outcome?
#### Consistency
Consistency means that data written to the database is guaranteed to be valid data, in terms of the database schema. The database or other data source must always be in a consistent state. One example of an inconsistent state would be a field in which half of the data is written before an operation aborts. A consistent state would be if all the data were written, or the write were rolled back when it could not be completed.
#### Isolation
Isolation means that data being operated on by a transaction must be locked before modification, to prevent processes outside the scope of the transaction from modifying the data.
#### Durability
Durability means that in the event of an external failure after transaction members have been instructed to commit, all members will be able to continue committing the transaction when the failure is resolved. This failure can be related to hardware, software, network, or any other involved system.
