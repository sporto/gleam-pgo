# Changelog

## v0.12.0 - 2024-07-03

- Added the `transaction` function and `TransactionError` type.

## v0.11.0 - 2024-06-22

- Provided functions for handling date values. The `date` function
  coerces a `#(Int, Int, Int)` value representing `#(year, month, day)` into a
  `Value`. The `decode_date` function can be used to decode a dynamic value
  returned from the database as a date in the same tuple format.

## v0.10.0 - 2024-05-31

- The `uri_config` function now accepts the `postgresql://` scheme as well as
  the `postgres://` scheme.

## v0.9.0 - 2024-05-20

- Provided functions for handling timestamp values. The `timestamp` function
  coerces a `#(#(Int, Int, Int), #(Int, Int, Int))` value representing
  `#(#(year, month, day), #(hour, minute, second))` into a `Value`. The
  `decode_timestamp` function can be used to decode a dynamic value returned from
  the database as a timestamp in the same nested tuple format.

## v0.8.0 - 2024-05-20

- Added `array` column handling, accepting a `List` as value.

## v0.7.0 - 2024-04-05

- The password is now optional in the `url_config` function, defaulting to no
  password if none is given.

## v0.6.1 - 2024-01-16

- Relaxed the stdlib version constraint.

## v0.6.0 - 2023-11-06

- Updated for Gleam v0.32.0.

## v0.5.0 - 2023-08-03

- Updated for Gleam v0.30.0.

## v0.4.1 - 2023-03-02

- Updated for Gleam v0.27.0.

## v0.4.0 - 2022-06-12

- IPv6 is now supported through a config option.

## v0.3.0 - 2022-02-17

- Added the `ConnectionUnavailable` error variant.

## v0.2.0 - 2022-01-26

- Migrate to the Gleam build tool.
- API redesigned.

## v0.1.1 - 2020-11-26

- Dependencies updates and versions relaxed.

## v0.1.0 - 2020-08-24

- Initial release.
