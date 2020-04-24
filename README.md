# Merkle-tree

A binary tree of one-time signatures known as merkle tree. Often used in distributed systems such as Git, Cassandra or Bitcoin for efficiently summarizing sets of data.

A binary tree originally developed to authenticate a large number of public keys with a single value, namely the root of the tree. The merkle root is usually available publicly. Each node in the tree contains a cryptographic hash of node values of its children. The N values/messages that need to be authenticated are placed at the N leaves of the tree. A leaf can store an arbitrary value, usually a public authentication key, that is a cryptographic hash of the value that needs to be authenticated. A leaf can be then verified by publicly available merkle tree root value and its authentication path.
