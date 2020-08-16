# Lavalink

`twilight-mention` is a utility crate to mention [`twilight-model`] types.

With this library, you can create mentions for various types, such as users,
emojis, roles, members, or channels.

### Installation

This library requires at least Rust 1.45.0+.

Add the following to your `Cargo.toml`:

```toml
twilight-mention = { branch = "trunk", git = "https://github.com/twilight-rs/twilight" }
```

### Examples

Create a mention formatter for a user ID, and then format it in a message:

```rust
use twilight_mention::Mention;
use twilight_model::id::UserId;

let user_id = UserId(123);
let message = format!("Hey there, {}!", user_id.mention());
```

### Links

*source*: <https://github.com/twilight-rs/twilight/tree/trunk/utils/mention>

*docs*: <https://twilight-rs.github.io/twilight/twilight_mention/index.html>

*crates.io*: <https://crates.io/crates/twilight-mention>

[`twilight-model`]: ../section_1_model.html