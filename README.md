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

## Flow:
ADC IR values go about that:
- ~1700 on the table
- ~1770 nicely covered with hand
- ~2160 when the IR is missing (not wired)
- ~1660 with phone lighter level 5 touching IR
