---
title: 'pganalyze Log Insights'
backlink_href: /docs
backlink_title: 'Documentation'
---

![](setup/log_insights_screenshot.png)

Welcome to pganalyze **Log Insights** - the best way to monitor and analyze your
PostgreSQL log files, and give you insights into how to tune your database better,
or to explain why your database might be slow at a given moment.

## Setting up Log Insights

To start, follow the platform-specific setup steps:

* [Amazon RDS & Amazon Aurora](/docs/log-insights/setup/amazon-rds)
* [Azure Database for PostgreSQL](/docs/log-insights/setup/azure-database)
* [Google Cloud SQL](/docs/log-insights/setup/google-cloud-sql)
* [Heroku Postgres](/docs/log-insights/setup/heroku-postgres)
* [Self-Managed Server](/docs/log-insights/setup/self-managed)

## Making the most of Log Insights

After you have completed the initial setup of Log Insights, we recommend two more steps:

* [Tune Postgres logging parameters](/docs/log-insights/setup/tuning-log-config-settings)<br />Enable additional important log events for your Postgres server.
* [Set up automatic EXPLAIN plan collection](/docs/explain/setup)<br />Automatically get detailed EXPLAIN plans for slow queries in your system.

## Log Events

Internally in pganalyze each log line gets assigned one of the event types below, to uniquely identify the circumstances under which such an event was triggered.

These classifications are then used for alerting and filtering purposes, and allow you to quickly find the corresponding documentation for an event.

### Log Event Categories:

* [Server](/docs/log-insights/server)
* [Connections](/docs/log-insights/connections)
* [WAL & Checkpoints](/docs/log-insights/wal-checkpoints)
* [Autovacuum](/docs/log-insights/autovacuum)
* [Locks](/docs/log-insights/locks)
* [Statements](/docs/log-insights/statements)
* [Standby Servers](/docs/log-insights/standby)
* [Constraint Violations](/docs/log-insights/constraint-violations)
* [Application / User Errors](/docs/log-insights/app-errors)

### Log event types in comparison to SQLSTATE

Those familiar with [SQL error codes](https://www.postgresql.org/docs/current/static/errcodes-appendix.html) (SQLSTATE) might ask themselves: Why invent yet another log line categorization system?

In our experience working with Postgres logs, whilst the SQL error codes in logs are useful (if they are being output), they unfortunately cover less than 50% of the useful log events we encountered.

Where available this documentation includes a reference to the corresponding SQLSTATE code, so you can match it up.
