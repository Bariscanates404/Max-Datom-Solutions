# Max-Datom-Solutions

Personal solutions to a numbered series of Datomic query exercises, written in Clojure.

## What it is

One Clojure file per level (`level-3` to `level-12`). Each file contains the exercise query first and, after a `solution --->` marker, the answer: a Datomic Datalog query run with `datomic.client.api/q` against a `db` value.

## Why it exists

Practice for Datomic Datalog (find/where clauses, `count`, `not`, `pull`). The origin of the exercise series is not documented in the repo, and the namespace `max-datom.connections` that provides `db` is not included, so the files are not runnable on their own.

## Contents

| Path | What it is |
|---|---|
| `level-3`, `level-4` | Simple `:find` queries over author and book attributes |
| `level-5` to `level-9` | Further query exercises with solutions |
| `level-10` | Lookup by `:user/id` and count of that user's posts |
| `level-11` | Per-user post counts using `not` (posts without dislikes) |
| `level-12` | `pull` of post authors plus a small helper function |

The files have no `.clj` extension.

## How to run

No manifest (`deps.edn` etc.) is included. To try a query you need a Clojure REPL with the Datomic client library (`datomic.client.api`) and your own `max-datom.connections` namespace that defines `db`; paste the query from a level file into the REPL.

## Tech stack

Clojure, Datomic (client API), Datalog.

## Status

Archived exercises. Last commit 2023-05-30, 11 commits.

## Related repos

None evident.
