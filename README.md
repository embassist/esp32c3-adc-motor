## Firmware:
### NOTE: keep comments on top of the code, removal seems to lead to
```
#[instability::unstable]
     |     ------------------------ private method defined here
```
- clone esp-hal
- replace `embassy_hello_world.rs` example with `main.rs`
- ```shell
    cargo xtask run-example esp-hal esp32c3 embassy_hello_world
  ```

## Hardware:
- esp32c3
- IR photoresistor
### Wiring:
- IR+ -> esp pin4/5
- IR- -> esp gnd
