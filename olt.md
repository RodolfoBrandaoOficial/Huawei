# Huawei OLT Commands 💼

This repository contains a list of useful commands for configuring and managing Huawei OLT (Optical Line Terminal) devices. These commands are helpful for network administrators and engineers working with Huawei OLT equipment. 🌐

## Version and Patch Information 📌

- Display current software version: `display version` 📋
- Display all patches: `display patch all` 🛠️

## Configuration ⚙️

- Display current configuration: `display current-configuration` 📄
- Save configuration: `save` 💾
- Display specific configuration sections:
  - VLAN configuration: `display current-configuration | section vlan` 🌐
  - GPON configuration: `display current-configuration | section gpon` 📡
  - BTV configuration: `display current-configuration | section btv` 📺
  - Device configuration: `display current-configuration | section device` 💻
  - Post configuration: `display current-configuration | section post` 📮
  - ABS configuration: `display current-configuration | section abs` 🔒
  - Public configuration: `display current-configuration | section public` 🌐
  - Global configuration: `display current-configuration | section global` 🌍

## Search Configuration 🔍

- Search for specific text in the configuration: `display current-configuration | include <text>` 🧐

## Statistics 📊

- Display board information: `display board 0` 🧰
- Display specific board information: `display board 0/5` 🧰
- Display CPU information: `display cpu 0/5` 💻
- Display resource information: `display resource` 📈
- Display security configuration: `display security config` 🔒
- Display temperature information: `display temperature` 🌡️
- Display GPON statistics: `display gpon statistics ethernet 0/5 0` 📈

## Specific Card and Port Information 📟

- MCUD GE0 information: 
  - Enter configuration mode: `config` ⚙️
  - Access MCUD GE0 interface: `interface mcu 0/2` 📟
  - Display DDM information: `display port ddm-info 0` 📊
  - Display traffic information: `display port traffic 0` 📈

- SCUN GE0 port information:
  - Enter configuration mode: `config` ⚙️
  - Access SCUN GE0 interface: `interface scu 0/8` 📟
  - Display DDM information: `display port ddm-info 0` 📊
  - Display traffic information: `display port traffic 0` 📈

## Alarms ⚠️

- Display active alarms: `display alarm active all` 🚨

## Time and NTP ⏰

- Display time information: `display time` 🕰️
- Display timezone information: `display timezone` 🌍
- Display daylight saving time information: `display time dst` ☀️
- Display time-stamp information: `display time time-stamp` 📅
- Display time range information: `display time-range` 🕰️
- Display NTP service information: `display ntp-service` 🌐

## Security 🔒

- Example of DoS protection configuration:
  - Display control packet rate: `display security anti-dos control-packet rate 0/5/0` 🛡️
  - Display DoS blacklist: `display security dos-blacklist all` 🚫

## MAC and ARP 🌐

- Display MAC addresses:
  - By VLAN: `display mac-address vlan 1501` 📶
  - For a specific service port: `display mac-address service-port 12` 📶
  - By port: `display mac-address port 0/5/0` 📶
  - All MAC addresses: `display mac-address all` 📶
  - Search for a specific MAC address: `display mac-address all | include 000c-29b9-3331` 📶

- Clear MAC address:
  - Example: `undo mac-address mac 000c-29b9-3331 vlan 1501` 🗑️

- Display ARP table: `display arp all` 🌐

## CPU Control ⚙️

- Configure CPU control parameters: `display cpu-overload-control parameter` 🧑‍💻
- Adjust CPU control factor: `cpu-overload-control parameter adjustfactor 20` 🔄

## Console Output 📢

- Enable alarms output on the console: `alarm output all` 🔊
- Disable alarms output on the console: `undo alarm output all` 🔕

## Logs 📜

- Display various logs:
  - All logs: `display log all` 📜
  - CLI logs: `display log cli` 💬
  - Failure logs: `display log failure` ❌
  - Index logs: `display log index` 📊
  - Memory logs: `display log memory` 🧠
  - Name logs: `display log name` 📜
  - Security logs: `display log security` 🔒
  - SNMP logs: `display log snmp` 📡

- Manage syslog:
  - Disable syslog: `syslog disable` 🚫
  - Enable syslog: `syslog enable` ✅
  - Configure syslog output: `syslog output` 📤
  - Synchronize syslog: `syslog sync` 🔄

## Additional Commands 🛠️

- Other useful commands like `cls`, `display bandwidth`, `display alarm`, `display autosave configuration`, `display baudrate`, `display board number`, and more.

- GPON-related commands such as `interface gpon`, `display ont alarm-profile`, `display ont alarm-state`, `display ont autofind`, etc.

Feel free to explore and use these commands as needed for managing Huawei OLT devices. 🚀









Huawei MA56xx OLT Command Lists

Exibição da versão atual e patch do OLT:

shell
Copy code
display version
display patch all
Visualização da configuração atual:

shell
Copy code
display current-configuration
Salvar a configuração:

shell
Copy code
save
Visualização da configuração atual em seções específicas:

shell
Copy code
display current-configuration | section vlan
display current-configuration | section gpon
display current-configuration | section btv
display current-configuration | section device
display current-configuration | section post
display current-configuration | section abs
display current-configuration | section public
display current-configuration | section global
Visualização da configuração atual em que um texto específico é encontrado:

shell
Copy code
display current-configuration | include 485754431CBD8333
Exemplo de visualização de várias estatísticas:

shell
Copy code
display board 0
display board 0/5
display cpu 0/5
display resource
display security config
display temperature
display gpon statistics ethernet 0/5 0
Informações sobre o cartão MCUD GE0 do MA5608T:

shell
Copy code
MA5608T#config
MA5608T(config)#interface mcu 0/2
MA5608T(config-if-mcu-0/2)#display port ddm-info 0
MA5608T(config-if-mcu-0/2)#display port traffic 0
Informações sobre a porta GE0 do cartão SCUN do MA5683T:

shell
Copy code
MA5683T#config
MA5683T(config)#interface scu 0/8
MA5683T(config-if-scu-0/8)#display port ddm-info 0
MA5683T(config-if-scu-0/8)#display port traffic 0
Exibição de alarmes ativos:

shell
Copy code
display alarm active all
Informações de tempo:

shell
Copy code
display time
display timezone
display time dst
display time time-stamp
display time-range
display ntp-service
Exemplo de configuração de proteção contra DoS:

shell
Copy code
display security anti-dos control-packet rate 0/5/0
display security dos-blacklist all
Exibição de endereços MAC:

shell
Copy code
display mac-address vlan 1501
display mac-address service-port 12
display mac-address port 0/5/0
display mac-address all
display mac-address all | include 000c-29b9-3331
Limpar endereço MAC:

shell
Copy code
Gponsolution-MA5683T#config
Gponsolution-MA5683T(config)#undo mac-address mac 000c-29b9-3331 vlan 1501
Exibição de endereços ARP:

shell
Copy code
display arp all
Configuração de sobrecarga da CPU de controle:

shell
Copy code
display cpu-overload-control parameter
cpu-overload-control parameter adjustfactor 20
Habilitar / desabilitar a exibição de alarmes no console:

shell
Copy code
alarm output all
undo alarm output all
Configuração e visualização de logs:

shell
Copy code
display log all
display log cli
display log failure
display log index
display log memory
display log name
display log security
display log snmp
display loghost
log modify operating
log modify security
loghost activate
loghost add
loghost deactivate
loghost delete
display syslog
syslog disable
syslog enable
syslog output
syslog sync
Outros comandos:

shell
Copy code
cls
display bandwidth
display alarm
display autosave configuration
display baudrate
display board number
Comandos relacionados ao GPON:

shell
Copy code
interface gpon
display ont alarm-profile
display ont alarm-state
display ont autofind
