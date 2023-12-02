# Configuration of DNS Server with BIND

This project provides a guide and configuration files to set up a DNS server using BIND (Berkeley Internet Name Domain) in a Linux-based environment. This DNS server is designed to manage domain name resolution within a local network.

## Project Structure

* sistema.sol: Example zone file for the sistema.sol domain.
* sistema.sol.rev: Example reverse zone file for the sistema.sol domain.
* named.conf.options: Main configuration for BIND with global configuration options

## Key Configurations

- named.conf.options.

The named.conf.options file contains the main configurations for the DNS server, including:

* Definition of forwarders to forward unresolved queries to external DNS servers.
* Configuration of recursion to allow recursive DNS query resolution.
* dnssec-validation enabled to validate the security of DNS responses.

## Zones

* sistema.sol: Configuration of the primary zone for the sistema.sol domain.
* sistema.sol.rev: Configuration of the reverse zone for the sistema.sol domain.

## Installation and Usage Steps

1) Clone the Repository: git clone https://github.com/jdgc5/dns-server-bind.git
2) Edit Configurations: Customize the configuration files according to your environment.
3) Use Vagrant up
4) Connect and configure your servers
5) Check Status: Use systemctl status bind9 to ensure BIND is running correctly.

## Contribution
Feel free to contribute to the project by suggesting improvements or corrections to the configurations. Open an issue to discuss changes or submit a pull request.

## Author
Jose David Garcia Corzo
Contact: dgc105@gmail.com
