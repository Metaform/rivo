![Rivo](/assets/rivo.logo.svg)

Rivo is an implementation of the
[Structured Task Collaboration](https://github.com/Metaform/dsaf-specs/blob/main/specs/stc/task-collaboration.md)
protocol (STC). It implements the Task Collaboration API for one or more participant contexts. An application that
implements a use case profile attaches to Rivo through a REST API and application events.

## Repository layout

| Path         | Contents                                                                       |
|--------------|--------------------------------------------------------------------------------|
| `rivo-core/` | The model, services, processors, and dispatcher, with no database or transport |
| `docs/`      | Runtime documentation                                                          |

## Running tests

```bash
cargo test --all-features
```

[cargo-nextest](https://nexte.st/) is supported and recommended; `.config/nextest.toml` tunes it for container-based
tests:

```bash
cargo install cargo-nextest --locked
cargo nextest run --all-features
```

## License

[Apache-2.0](LICENSE)
