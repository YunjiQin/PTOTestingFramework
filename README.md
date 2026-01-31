# PTO Testing Framework

A general-purpose integration testing framework designed to perform fuzz testing between different frontends and backends.

## Getting Started

This repository uses git submodules. Clone with the `--recursive` flag to fetch all dependencies:

```bash
git clone --recursive https://github.com/<your-org>/pto-testing-framework.git
```

If you have already cloned the repository without `--recursive`, run:

```bash
git submodule update --init --recursive
```

## Architecture

The framework decouples frontends and backends, allowing any frontend to be tested against any backend via fuzz testing.

### Frontend

- [pypto](https://github.com/hw-native-sys/pypto) — located at `3rdparty/pypto`

### Backend

- [simpler](https://github.com/ChaoWao/simpler) — located at `3rdparty/simpler`

## Testing

This framework uses **fuzz testing** to validate the integration between frontends and backends.