# ansible-role-rss-bridge

[![CI](https://github.com/vvision/ansible-role-rss-bridge/workflows/CI/badge.svg?event=push)](https://github.com/vvision/ansible-role-rss-bridge/actions?query=workflow%3ACI)

Ansible role to install rss-bridge.

## Requirements

A webserver of your choice to serve files.

## Role Variables

    php_version: "7.4"

PHP version for dependencies.

    rss_bridge_zip_url: https://github.com/RSS-Bridge/rss-bridge/archive/refs/tags

Where to find the zip package.

    rss_bridge_zip_name: "2021-04-25"

Name of zip.

    rss_bridge_file_owner: www-data

Owner of files.

    rss_bridge_file_group: www-data

Group of files.
    
    rss_bridge_single_user: true

Whether to enable builtin authentification for a single user.

    rss_bridge_username: root

Username for single user mode.

    rss_bridge_password: toor

Password for single user mode
    
    rss_bridge_bridges_list: [
    'Facebook',
    'Instagram',
    'Twitter',
    'Youtube'
    ]

List of bridges to whitelist. See full list [here](https://github.com/RSS-Bridge/rss-bridge/tree/master/bridges).

## Dependencies

* geerlingguy.php-versions
* geerlingguy.php

## License

MIT

## Author Information

This role was created in 2021 by Victor Voisin.
