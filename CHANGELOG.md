# Textfsm-aos release notes

## [1.0.0] - 2022-05-12

### Added CLI commands

- aos8 - `show vlan members` [#47](https://github.com/jefvantongerloo/textfsm-aos/pull/47)

### Changed

- parser - remove scrapli dependency by using native TextFSM module [#45](https://github.com/jefvantongerloo/textfsm-aos/pull/45)
- migrate packaging to Poetry [#48](https://github.com/jefvantongerloo/textfsm-aos/pull/45)

### Fixed

- aos8 - `show unp user` fix ipv6 in user_ip [#46](https://github.com/jefvantongerloo/textfsm-aos/pull/46)
- pytest - test `template_index_names`, fix empty list return [#44](https://github.com/jefvantongerloo/textfsm-aos/pull/44)

## [0.3.0] - 2022-04-11

### Added CLI commands

- aos6 - `show 802.1x users unp` [#30](https://github.com/jefvantongerloo/textfsm-aos/pull/30)
- aos8 - `history` [#32](https://github.com/jefvantongerloo/textfsm-aos/pull/32) by [@BennyE](https://github.com/BennyE)
- aos8 - `show health` [#24](https://github.com/jefvantongerloo/textfsm-aos/pull/24) by [@BennyE](https://github.com/BennyE)
- aos8 - `show ip interface` [#20](https://github.com/jefvantongerloo/textfsm-aos/pull/20) by [@BennyE](https://github.com/BennyE)
- aos8 - `show ip routes` [#21](https://github.com/jefvantongerloo/textfsm-aos/pull/21) by [@BennyE](https://github.com/BennyE)
- aos8 - `show interfaces status` [#27](https://github.com/jefvantongerloo/textfsm-aos/pull/27) by [@BennyE](https://github.com/BennyE)
- aos8 - `show transceivers` [#23](https://github.com/jefvantongerloo/textfsm-aos/pull/23) by [@BennyE](https://github.com/BennyE)
- pytest - test if command count matches textfsm template count [#29](https://github.com/jefvantongerloo/textfsm-aos/pull/29)
- pytest - test if command names matches testfsm template names [#29](https://github.com/jefvantongerloo/textfsm-aos/pull/29)

### Fixed

- aos6 - `show lldp remote-system` fix `remote port default vlan` value [#41](https://github.com/jefvantongerloo/textfsm-aos/pull/41)
- aos6 - `show mac address-table` fix trailing spaces and empty protocol with `---` placeholder [#39](https://github.com/jefvantongerloo/textfsm-aos/pull/39)
- aos8 - `show cmm` fix missing ',' at end of line on fpga parameters [#3](https://github.com/jefvantongerloo/textfsm-aos/pull/35)
- aos8 - `show interfaces status` fix add 21000 configured speed [#42](https://github.com/jefvantongerloo/textfsm-aos/pull/42)
- aos8 - `show ip routes` fix whitespace between days and hours [#40](https://github.com/jefvantongerloo/textfsm-aos/pull/40)
- aos8 - `show log events` catch space in time instead of '0', for example `2022 Apr  7 17: 8: 5.306` [#37](https://github.com/jefvantongerloo/textfsm-aos/pull/37)
- aos8 - `show log events` ':' in log_description value for example `Authentication failure detected: user admin` [#43](https://github.com/jefvantongerloo/textfsm-aos/pull/43)
- aos8 - `show mac-learning` missing trailing whitespace in output causes parsing error [#5](https://github.com/jefvantongerloo/textfsm-aos/pull/5)
- aos8 - `show unp user` catch missing trailing whitespace [#36](https://github.com/jefvantongerloo/textfsm-aos/pull/36)
- aos8 - `show snmp community-map` fix empty username field value [#38](https://github.com/jefvantongerloo/textfsm-aos/pull/38)

### New contributors
[@FlorianHeigl](https://github.com/FlorianHeigl) first contribution [https://github.com/jefvantongerloo/textfsm-aos/pull/30](https://github.com/jefvantongerloo/textfsm-aos/pull/30)

## [0.2.0] - 2022-03-14

### Added CLI commands

- aos6 - `show command-log` [#5](https://github.com/jefvantongerloo/textfsm-aos/pull/5)
- aos6 - `show running-directory` [#8](https://github.com/jefvantongerloo/textfsm-aos/pull/8) by [@BennyE](https://github.com/BennyE)
- aos6 - `show snmp station` [#17](https://github.com/jefvantongerloo/textfsm-aos/pull/17) by [@BennyE](https://github.com/BennyE)
- aos8 - `show chassis` [#6](https://github.com/jefvantongerloo/textfsm-aos/pull/6)
- aos8 - `show cmm` [#12](https://github.com/jefvantongerloo/textfsm-aos/pull/12)
- aos8 - `show command-log` [#4](https://github.com/jefvantongerloo/textfsm-aos/pull/4)
- aos8 - `show log events` [#14](https://github.com/jefvantongerloo/textfsm-aos/pull/14)
- aos8 - `show ntp server status` [#16](https://github.com/jefvantongerloo/textfsm-aos/pull/16) by [@BennyE](https://github.com/BennyE)
- aos8 - `show mac-learning` [#15](https://github.com/jefvantongerloo/textfsm-aos/pull/15) by [@BennyE](https://github.com/BennyE)
- aos8 - `show microcode` [#2](https://github.com/jefvantongerloo/textfsm-aos/pull/2)
- aos8 - `show snmp community-map` [#18](https://github.com/jefvantongerloo/textfsm-aos/pull/18) by [@BennyE](https://github.com/BennyE)
- aos8 - `show system` [#3](https://github.com/jefvantongerloo/textfsm-aos/pull/3)
- aos8 - `show unp user` [#11](https://github.com/jefvantongerloo/textfsm-aos/pull/11)
- aos8 - `show user` [#13](https://github.com/jefvantongerloo/textfsm-aos/pull/13) by [@BennyE](https://github.com/BennyE)
- aos8 - `show vlan` [#7](https://github.com/jefvantongerloo/textfsm-aos/pull/7) by [@BennyE](https://github.com/BennyE)

### Fixed

- aos6 - `show health` asterisk in current value not captured [#10](https://github.com/jefvantongerloo/textfsm-aos/pull/10)
- aos8 - `show cmm` os6560 only first chassis captured [#19](https://github.com/jefvantongerloo/textfsm-aos/pull/19)

### New contributors

- [@BennyE](https://github.com/BennyE) first contribution [https://github.com/jefvantongerloo/textfsm-aos/pull/7](https://github.com/jefvantongerloo/textfsm-aos/pull/7)

## [0.1.0] - 2022-02-23

### Added CLI commands

- aos6 - `show 802.1x users`
- aos6 - `show 802.1x non-supplicant`
- aos6 - `show 802.1x non-supplicant unp`
- aos6 - `show chassis`
- aos6 - `show health`
- aos6 - `show history`
- aos6 - `show interfaces status`
- aos6 - `show ip interface`
- aos6 - `show ip route`
- aos6 - `show lldp remote-system`
- aos6 - `show mac-address-table`
- aos6 - `show microcode`
- aos6 - `show ntp server status`
- aos6 - `show user`
- aos6 - `show snmp station`
- aos6 - `show snmp community map`
- aos6 - `show system`
- aos6 - `show vlan`
- aos6 - `show vlan port mobile`
