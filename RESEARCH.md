# RESEARCH

## OLTP

- MongoDB Atlas standalone binary 
- Data sharding with automatic\

## Materilized

- 

## LSM Backed by Object Store

- SlateDB - For OLTP use
- Tonbo - For OLAP use

## Raw Broker 

- Gazette ..
- Flow + Estuary

## Git-like for Object Store

- LakeFS

## Streaming / DataFlow

- RisingWave - 
- Real-time fraud - Arroyo - https://www.arroyo.dev/
- Fluvio 

## Data Catalog

- Iceberg Catalog - 

## Data Orchestration

- PeerDB - into ClickHouse ...
- 

## Time-Series

- HoraeDB - 

## PostGres Plugin

- Search inside PG - peerDB?
- DuckDB inside PG - 
- VectorDB inside PG? - 

## Combine data

- GlareDB - 

## Modern flow

- Fraud uses Cloudflare features (global)
- Global Connect via Cloudflare ..
- Operational data might uses Dynamic NoSQL, NewSQL - MongoDB; project to Postgres
- Postgres will have Facts Table + Temporal Table (starts monthly, then weekly, then daily) + snapshots
- PG to S3 - use PeerDB native replay to S3 in Gazette form
- Project from Gazette to raw snapshots controlled by Data Owners; foundation hierarchy 
- Postgres in Operator - DuckDB for easy exploration; shared cache + read-on;ly
- LakeFS will take from Iceberg; transform from raw to Bronze, Silver, Gold
- SQLMesh will participate with the Orchestration + Promotion
- Join multiple row + columnar for materilized views .. continuous .. send off 
- Analysts will be responsible for intermediate derivation .. SQLMesh for lineage
- Feature Engineering from structured final data
- Finance ledger from immutable snapshots
- Data will be Reverse ETL for other use like marketing
- Data Tokenizing Service
