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




# Meu Projeto Incrível :rocket:

Bem-vindo ao meu projeto incrível! Este projeto faz [descrição do projeto] e [outras informações interessantes].

## Recursos

- :heavy_check_mark: Recurso 1
- :bulb: Recurso 2
- :chart_with_upwards_trend: Recurso 3

## Como Começar

Siga estas etapas para começar com o projeto:

1. :fork_and_knife: Faça um fork deste repositório
2. :arrow_down: Clone o repositório para a sua máquina local
3. :computer: Execute `npm install` para instalar as dependências
4. :rocket: Execute `npm start` para iniciar o aplicativo

## Contribuindo

Sinta-se à vontade para contribuir com este projeto. Se você deseja adicionar novos recursos ou corrigir problemas, siga estas etapas:

1. :fork_and_knife: Faça um fork deste repositório
2. :arrow_down: Clone o repositório para a sua máquina local
3. :rocket: Crie uma nova branch para a sua contribuição (`git checkout -b minha-contribuicao`)
4. :pencil: Faça suas alterações e faça commit (`git commit -m 'Adicionei um novo recurso'`)
5. :arrow_up: Envie suas alterações para o seu fork (`git push origin minha-contribuicao`)
6. :octocat: Abra um pull request neste repositório

## Contato

Se você tiver alguma dúvida ou precisar de assistência, entre em contato conosco em [seu-email@example.com].

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE.md](LICENSE.md) para obter detalhes.

:sunglasses: Divirta-se codificando! :computer:

