<div align="center">

![Logo](https://raw.githubusercontent.com/francis-du/iotdb-rs/main/iotdb-rs.png)

<h1>iotdb-cli</h1>
<h3>(WIP) Apache IotDB CLI Client written in Rust</h3>

[![License](https://img.shields.io/badge/license-Apache%202.0-blue?style=flat-square&color=%23E5531A)](https://github.com/francis-du/iotdb-cli/blob/main/LICENSE)
[![Rust Build](https://img.shields.io/github/workflow/status/francis-du/iotdb-cli/cargo-test?label=build&style=flat-square)](https://github.com/francis-du/iotdb-cli/actions?query=workflow%3Acargo-test)
[![Crates Publish](https://img.shields.io/github/workflow/status/francis-du/iotdb-cli/cargo-publish?label=publish&style=flat-square)](https://github.com/francis-du/iotdb-cli/actions?query=workflow%3Acargo-publish)

</div>

---

## Installation

```shell
cargo install iotdb-cli
```

## Usage

```shell
iotdb -h
```

```shell
▀██▀  ▄▄█▀▀██   █▀▀██▀▀█ ▀██▀▀█▄   ▀██▀▀█▄
 ██  ▄█▀    ██     ██     ██   ██   ██   ██
 ██  ██      ██    ██     ██    ██  ██▀▀▀█▄
 ██  ▀█▄     ██    ██     ██    ██  ██    ██
▄██▄  ▀▀█▄▄▄█▀    ▄██▄   ▄██▄▄▄█▀  ▄██▄▄▄█▀      0.0.1

USAGE:
    iotdb-cli [FLAGS] [OPTIONS]

FLAGS:
    -d, --debug      Enable debug mode
    -h, --help       Prints help information
    -V, --version    Prints version information

OPTIONS:
        --endpoint <endpoint>      Endpoint
    -H, --host <host>              Server host name
        --log-level <log-level>    Logger level
    -p, --password <password>      User password
    -P, --port <port>              Server port
    -u, --user <user>              User name
```

## Run

```shell
iotdb -u root -p root --endpoint 127.0.0.1:6667 -t UTC+8

▀██▀  ▄▄█▀▀██   █▀▀██▀▀█ ▀██▀▀█▄   ▀██▀▀█▄
 ██  ▄█▀    ██     ██     ██   ██   ██   ██
 ██  ██      ██    ██     ██    ██  ██▀▀▀█▄
 ██  ▀█▄     ██    ██     ██    ██  ██    ██
▄██▄  ▀▀█▄▄▄█▀    ▄██▄   ▄██▄▄▄█▀  ▄██▄▄▄█▀     

Connect server: 127.0.0.1:6667
Version: 0.0.1
IOTDB#> SHOW STORAGE GROUP
+---------------+
| storage group |
+===============+
| root.ln       |
+---------------+
| root.sg1      |
+---------------+
IOTDB#> 
```