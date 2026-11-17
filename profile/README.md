# DBinvent

Chicago based deep tech startup since 2019, building
[YT Cluster](https://www.dbinvent.com/cluster/): vanilla PostgreSQL plus an extension, a
cluster with no dedicated master. Your database becomes a node where it already sits - no
data transfer, no code change, no vendor lock.

## Open source

| Repository | What it is |
|---|---|
| [yt-cluster-lite](https://github.com/DBinvent/yt-cluster-lite) | **YT Cluster Lite**, the open part of YT Cluster (MIT): the protocol the levels of a cluster hierarchy use to exchange rows, the PostgreSQL extension, and YT lite - a node for one database that links to a cluster and syncs the tables you choose both ways: beside PostgreSQL, inside SQLite, or inside your application on Turso |
| [yt-cluster-tests](https://github.com/DBinvent/yt-cluster-tests) | YT Cluster's integration tests: the nightly suites, Jepsen, the security gate (Trivy, `cargo audit`) and the SBOMs of each release |
| [sge](https://github.com/DBinvent/sge) | **Schema Guard Enterprise**, schema management for PostgreSQL (MIT): versioned SQL scripts tracked like Flyway, a declarative schema with a `plan` phase like Terraform, dry runs, snapshots and loads - on [crates.io](https://crates.io/crates/schema_guard) and [Docker Hub](https://hub.docker.com/r/dbinvent/sge) |
| [signon](https://github.com/DBinvent/signon) | User management for Rust web back offices (MIT): registration, email verification, sessions, password reset, OAuth2, OIDC and SAML sign-in, notifications - on [crates.io](https://crates.io/crates/signon) |

## Read more

- [dbinvent.github.io](https://dbinvent.github.io/) - what we build and why:
  [Where rows live](https://dbinvent.github.io/where-rows-live.html) ·
  [YT Cluster vs PostgreSQL streaming replication](https://dbinvent.github.io/yt-cluster-performance.html) ·
  [30 pillars of YT Cluster](https://dbinvent.github.io/yt-cluster-pillars.html)
- [dbinvent.com](https://www.dbinvent.com) - the product, its guide and downloads
- [dbinvent/yt](https://hub.docker.com/r/dbinvent/yt) - a YT Cluster node in one container
