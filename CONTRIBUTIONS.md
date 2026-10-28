# Open-source contributions

Pull requests I have sent to projects I use, grouped by project. Statuses are updated from time to time.

Last updated: 2026-10-26.

## [Mamonsu](https://github.com/postgrespro/mamonsu)

PostgreSQL monitoring agent for Zabbix.

| Opened | Pull request | What it does | Status |
| --- | --- | --- | --- |
| 2026-08-27 | [#235](https://github.com/postgrespro/mamonsu/pull/235) | Optional TLS encryption (PSK or certificate) for the agent's connection to Zabbix; the unencrypted mode stays compatible. | Under review |

## [wintun-bindings](https://github.com/tun2proxy/wintun-bindings)

Rust bindings for the WireGuard Wintun driver on Windows.

| Opened | Pull request | What it does | Status |
| --- | --- | --- | --- |
| 2026-10-19 | [#22](https://github.com/tun2proxy/wintun-bindings/pull/22) | Checks the signature of `wintun.dll` before loading it, so none of its code runs before the check, and keeps the file locked until it is loaded. | Under review |
| 2026-10-19 | [#23](https://github.com/tun2proxy/wintun-bindings/pull/23) | Documents how the receive functions report a session shutdown, with a doctest showing how to tell it apart from other errors. | Under review |

## [tappers](https://github.com/pkts-rs/tappers)

Cross-platform TUN/TAP interfaces for Rust.

| Opened | Pull request | What it does | Status |
| --- | --- | --- | --- |
| 2026-10-19 | [#64](https://github.com/pkts-rs/tappers/pull/64) | Makes Wintun adapters work on Windows, loads `wintun.dll` safely with an optional signature check, adds `set_mtu()` on Windows, fixes descriptor leaks in release builds and makes Windows CI actually run the tests. | Under review |

## [netlink-packet-netfilter](https://github.com/rust-netlink/netlink-packet-netfilter)

Rust netlink packet types for the Linux netfilter subsystems, nf_tables included.

| Opened | Pull request | What it does | Status |
| --- | --- | --- | --- |
| 2026-10-23 | [#24](https://github.com/rust-netlink/netlink-packet-netfilter/pull/24) | Adds the `ct`, `limit`, `log` and `rt` nf_tables expressions, tested against netlink messages captured from `nft`. | Under review |

## [windows-service](https://github.com/mullvad/windows-service-rs)

A crate for implementing and managing Windows services.

| Opened | Pull request | What it does | Status |
| --- | --- | --- | --- |
| 2026-10-25 | [#148](https://github.com/mullvad/windows-service-rs/pull/148) | Adds `Service::set_start_type`, which changes only a service's start type without rebuilding its whole configuration. | Under review |
| 2026-10-25 | [#149](https://github.com/mullvad/windows-service-rs/pull/149) | Adds `Service::query_security_descriptor` and `set_security_descriptor` to read and write a service's security descriptor as an SDDL string. | Under review |

## [rpm](https://github.com/rpm-rs/rpm-rs)

A pure Rust library for reading, building and signing RPM packages.

| Opened | Pull request | What it does | Status |
| --- | --- | --- | --- |
| 2026-10-26 | [#378](https://github.com/rpm-rs/rpm-rs/pull/378) | Fixes a panic on inconsistent trigger tag arrays, stops signing without a signature backend from silently dropping signatures, applies librpm's signature header limits, reads headers in bounded chunks and adds a regression test with malformed headers. | Under review |

## [rpm-version](https://github.com/rpm-rs/rpm-version)

Rust library for RPM versions (NEVRA, EVR), sorted the same way as RPM.

| Opened | Pull request | What it does | Status |
| --- | --- | --- | --- |
| 2026-10-26 | [#1](https://github.com/rpm-rs/rpm-version/pull/1) | Makes `Evr` and `Nevra` equality and hashing agree with their ordering, so that ordered and hashed collections agree on which versions are duplicates, and fixes sortkeys of numeric segments longer than 255 digits. | Under review |
