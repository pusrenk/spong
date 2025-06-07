# spong
Sistem PengelOlaan uaNG

rust-service

current structure

```bash
my_project/
├── Cargo.toml
├── Cargo.lock
└── src/
    ├── main.rs          # Entry point (for binaries)
    ├── lib.rs           # Main library file
    ├── config.rs        # Configuration loading (e.g., using `config` or `dotenvy`)
    ├── routes/          # For web apps: route handlers
    │   ├── mod.rs       # for initiate module to the rust
    │   └── user.rs
    ├── handlers/        # Business logic
    │   ├── mod.rs
    │   └── user_handler.rs
    ├── models/          # Structs representing data models or DB schemas
    │   ├── mod.rs
    │   └── user.rs
    ├── services/        # Reusable services (e.g. auth, database)
    │   ├── mod.rs
    │   └── db.rs
    └── utils/           # Utility functions and helpers
        ├── mod.rs
        └── logger.rs
```