# mqtt-client-rs

An MQTT 3.1.1 client written in Rust.

## To run automated tests

Simply run `cargo test`.

The integration tests require an MQTT broker to run against, see the
instructions in `${REPO}/tests/integration_test.rs`.

## Run the test command-line app

Run `cargo run --bin mqttc` to print usage.

The test app requires an MQTT broker to run against, see the
instructions in `${REPO}/tests/integration_test.rs`.

Run `cargo run --bin mqttc -- --host localhost publish topic payload`
to publish payload `payload` to topic `topic`.

Run `RUST_LOG="info" cargo run --bin mqttc -- --host localhost subscribe topic`
to subscribe to topic `topic` and print any messages that are published to it.
