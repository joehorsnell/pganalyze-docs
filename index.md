---
title: 'Documentation'
---

* **[Installation Guide](/docs/install)**
  - [Troubleshooting](/docs/install/troubleshooting)

<hr />

* **[Log Insights](/docs/log-insights)**
  - [Initial setup](/docs/log-insights/setup)
      * [Amazon RDS & Amazon Aurora](/docs/log-insights/setup/amazon-rds)
      * [Azure Database for PostgreSQL](/docs/log-insights/setup/azure-database)
      * [Google Cloud SQL](/docs/log-insights/setup/google-cloud-sql)
      * [Heroku Postgres](/docs/log-insights/setup/heroku-postgres)
      * [Self-managed Postgres Server](/docs/log-insights/setup/self-managed)
  - [Tuning Log Config Settings](/docs/log-insights/setup/tuning-log-config-settings)
  - [Classifications](/docs/log-insights)
      * [Server](/docs/log-insights/server)
      * [Connections](/docs/log-insights/connections)
      * [WAL & Checkpoints](/docs/log-insights/wal-checkpoints)
      * [Autovacuum](/docs/log-insights/autovacuum)
      * [Locks](/docs/log-insights/locks)
      * [Statements](/docs/log-insights/statements)
      * [Standby Servers](/docs/log-insights/standby)
      * [Constraint Violations](/docs/log-insights/constraint-violations)
      * [Application / User Errors](/docs/log-insights/app-errors)

* **[EXPLAIN](/docs/explain)**
  - [Set up automatic EXPLAIN plan collection](/docs/explain/setup)
      * [auto_explain](/docs/explain/setup/auto_explain)
      * [Log-based EXPLAIN](/docs/explain/setup/log_explain)
  - [Insights](/docs/explain/insights)
      * [Disk Sort](/docs/explain/insights/disk-sort)
      * [Expensive](/docs/explain/insights/expensive)
      * [Hash Batches](/docs/explain/insights/hash-batches)
      * [Inefficient Index](/docs/explain/insights/inefficient-index)
      * [I/O Heavy](/docs/explain/insights/io-heavy)
      * [Large Offset](/docs/explain/insights/large-offset)
      * [Lossy Bitmaps](/docs/explain/insights/lossy-bitmaps)
      * [Mis-Estimate](/docs/explain/insights/mis-estimate)
      * [Slow Scan](/docs/explain/insights/slow-scan)
      * [Stale Stats](/docs/explain/insights/stale-stats)
  - [Scan nodes](/docs/explain/scan-nodes)
      * [Sequential Scan](/docs/explain/scan-nodes/sequential-scan)
      * [Index Scan](/docs/explain/scan-nodes/index-scan)
      * [Index-Only Scan](/docs/explain/scan-nodes/index-only-scan)
      * [Bitmap Heap Scan](/docs/explain/scan-nodes/bitmap-heap-scan)
      * [Bitmap Index Scan](/docs/explain/scan-nodes/bitmap-index-scan)
      * [CTE Scan](/docs/explain/scan-nodes/cte-scan)
      * [Custom Scan](/docs/explain/scan-nodes/custom-scan)
      * [Foreign Scan](/docs/explain/scan-nodes/foreign-scan)
      * [Function Scan](/docs/explain/scan-nodes/function-scan)
      * [Subquery Scan](/docs/explain/scan-nodes/subquery-scan)
      * [Table Sample Scan](/docs/explain/scan-nodes/table-sample-scan)
      * [Tid Scan](/docs/explain/scan-nodes/tid-scan)
      * [Values Scan](/docs/explain/scan-nodes/values-scan)
      * [Work Table Scan](/docs/explain/scan-nodes/work-table-scan)
  - [Join nodes](/docs/explain/join-nodes)
      * [Hash Join](/docs/explain/join-nodes/hash-join)
      * [Merge Join](/docs/explain/join-nodes/hash-join)
      * [Nested Loop](/docs/explain/join-nodes/nested-loop)
  - [Other nodes](/docs/explain/other-nodes)
      * [Aggregate](/docs/explain/other-nodes/aggregate)
      * [Append](/docs/explain/other-nodes/append)
      * [Bitmap And](/docs/explain/other-nodes/bitmap-and)
      * [Bitmap Or](/docs/explain/other-nodes/bitmap-or)
      * [Gather Merge](/docs/explain/other-nodes/gather-merge)
      * [Gather](/docs/explain/other-nodes/gather)
      * [Group](/docs/explain/other-nodes/group)
      * [Hash](/docs/explain/other-nodes/hash)
      * [Limit](/docs/explain/other-nodes/limit)
      * [Lock Rows](/docs/explain/other-nodes/lock-rows)
      * [Materialize](/docs/explain/other-nodes/materialize)
      * [Merge Append](/docs/explain/other-nodes/merge-append)
      * [Modify Table](/docs/explain/other-nodes/modify-table)
      * [Project Set](/docs/explain/other-nodes/project-set)
      * [Recursive Union](/docs/explain/other-nodes/recursive-union)
      * [Result](/docs/explain/other-nodes/result)
      * [SetOp](/docs/explain/other-nodes/set-op)
      * [Sort](/docs/explain/other-nodes/sort)
      * [Unique](/docs/explain/other-nodes/unique)
      * [Window Aggregate](/docs/explain/other-nodes/window-aggregate)

* **[Collector](/docs/collector)**
  - [Settings overview](/docs/collector/settings)

* **[Enterprise Edition](/docs/enterprise)**
  - [Initial Setup](/docs/enterprise/setup)
  - [Release Changelog](/docs/enterprise/releases)
  - [Log Insights Setup](/docs/enterprise/log-insights)
  - [Google Auth Setup](/docs/enterprise/google-auth)
  - [Upgrading to new releases](/docs/enterprise/upgrade)

* **[pganalyze GraphQL API](/docs/api)**
  - [Creating an API key](/docs/api/create-api-key)
  - [Queries](/docs/api/queries)
      * [getIssues - Get check-up issues and alerts](/docs/api/queries/getIssues)
      * [getQueryStats - Export query statistics](/docs/api/queries/getQueryStats)
  - [Mutations](/docs/api/mutations)
      * [addServer - Add a server to pganalyze Enterprise Edition](/docs/api/mutations/addServer)

<!--* **[Guides](/docs/guides)**
  - [Tuning checkpoint intervals to reduce I/O spikes](/docs/guides/tuning-checkpoint-intervals)
  - [Adjusting work_mem based on temporary file creation](/docs/guides/adjusting-work-mem)
  - [Exporting query statistics using the pganalyze API](/docs/guides/exporting-query-statistics)
  - [Monitoring Postgres locks using Log Insights](/docs/guides/monitoring-postgres-locks-using-log-insights)
-->

---

* [Permissions and Roles](/docs/permissions)
* [Open-Source Components](/docs/open_source_components)
