- Schema Design(Learn rules of relationships, rregullat e normalizimit)
- How would the schema adapt to feature requests
- Find out how a simple design would fail in a heavy workflow
- Implement performance optimization techniques (all of them Or at least have a plan for some of them for when the time comes they are needed)
- Investigate how the optimization techniques work down in technical detail


**Schema design**
	entities and attributes
		Entities: client, project, task, invoice, payment, time entry
	PK- unique identification of a row in a table
		unique, no null
		Natural primary key?
		2 PK in a table, unique tuples always
		does not need iteration to find PK
		Index vs PK?? (PK - which row is it, index - how can i find this efficiently. ==**research more**==)
		UUID vs int??? (integer and long string) - when would i use which
		Delete cascade or set null???? when would i use it
	FK - which row is this related to?
		referential integrity
		foreign-key constraints
		ON DELETE CASCADE
		ON DELETE RESTRICT
		ON DELETE SET NULL
		ON UPDATE
		orphan records
	Cardinality

Normalization

Schema evolution: "How would the schema adapt to feature requests?"

Find out how a simple design would fail in a heavy workflow

Performance optimization

Indexes

Query execution plans

Query planner and optimizer

Transactions and concurrency

Caching

Pagination

Database-level optimization



1: RD foundations
Goal: produce an ER diagram without guessing for a real life problem
	Relational model
	Tables, rows, columns
	Primary keys
	Foreign keys
	Candidate keys
	Constraints
	Relationships
	Cardinality
	ER diagrams
	Many-to-many relationships

2: normalizationn
Goal: if i have a bad table, realize what is wrong with it and why
	Data redundancy
	Insert/update/delete anomalies
	Functional dependencies
	Candidate keys
	1NF
	2NF
	3NF
	BCNF
	When normalization is useful
	When denormalization can be justified

3: schema evolution
Goal: if new feature is supposed to be added, be able to realize what changes are needed int he database
	Schema changes
	Migrations
	Data migrations
	Adding/removing columns
	Changing relationships
	Backward compatibility
	Expand/contract migrations
	Handling existing data
	Feature-driven schema changes

4: workload analysis
goal: to look at a simple database and predict where it will break as usage grows
	Read-heavy vs write-heavy
	Query frequency
	Data volume
	Query complexity
	Hot queries
	Hot rows
	Bottlenecks
	N+1 queries
	Large result sets
	Transaction contention

query performance
goal: investigate a slow query rather than just adding indexes
	Indexes
	B-trees
	Composite indexes
	Index selectivity
	Query planner
	EXPLAIN
	EXPLAIN ANALYZE
	Sequential scans
	Index scans
	Join algorithms
	Aggregation
	Sorting
	Pagination
	Query rewriting

6: concurrency and connection
goal: understand how 2 users changing same data can be safely done
	ACID
	Transactions
	Isolation
	Locks
	Deadlocks
	MVCC
	Concurrent writes
	Race conditions
	Atomic operations

7: higher level optimization
goal: know which technique is betetr for the case and what problem it actually solves
	Connection pooling
	Caching
	Cache invalidation
	Batching
	Materialized views
	Denormalization
	Partitioning
	Replication
	Read replicas
	Sharding

