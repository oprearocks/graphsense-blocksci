# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [0.4.2] - 2019-12-19
### Changed
- Removed exchange rates ingest from blocksci_export.py script (BlockSci uses the CoinDesk API, which supports only BTC)
- Updated utility script to check `block` and `exchange_rates` table
### Added
- Added scripts to ingest exchange rates from CoinDesk or CoinMarketCap
- Added script to obtain first block height on a specific date

## [0.4.1] - 2019-06-28
### Changed
- Multi-stage Dockerfile to reduce image size
### Added
- Added `--chunks` argparse argument
- Added doctests
### Removed
- Removed `tag` table from raw Cassandra schema ([GraphSense TagPacks](https://github.com/graphsense/graphsense-tagpacks))

## [0.4.0] - 2019-02-01
### Changed
- Fixed exchange rates bug (EUR/USD swapped)
- Refactored multiprocess ingests
- Specified fixed version of Python cassandra-driver
### Added
- Added coinjoin column to transaction table

## [0.3.3] - 2018-11-30
### Changed
- Updated BlockSci to v0.6 branch
