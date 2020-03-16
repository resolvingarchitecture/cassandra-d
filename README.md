# Cassandra-D
Decentralized Cassandra written in Rust!

Using Cassandra on [GitHub](https://github.com/apache/cassandra.git) for guidance.

Cassandra-D will be a highly-scalable partitioned row store. Rows will be organized into tables with a required primary key.

Partitioning means that Cassandra-D will be able to distribute your data across many peers in an application-transparent matter. Cassandra-D will automatically repartition as peers are added and removed from the trust ring.

Trust ring is a group of peers that have agreed to become a community sharing the load. They, together as a whole, get compensated
by end users purchasing persistence in BTC/XMR.

Row store means that like relational databases, Cassandra-D will organize data by rows and columns. The Cassandra-D Query Language (CDQL) will be very similar to SQL.

## Background

Cassandra-D is the middle of evaluating how best to decentralize Apache Cassandra. Cassandra is an amazing vehicle
for scaling persistence but mainly focused on using within a data-center like Amazon's AWS. Decentralized networks
today are largely focused on P2P communications like messengers as the infrastructure is not yet in place to support
large-scale Big Data type projects on decentralized networks. Cassandra-D aims to change this. And Rust is the perfect
language to ensure performance while maintaining memory safety.

## Requirements

* Rust 1.42
