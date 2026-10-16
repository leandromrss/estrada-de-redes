
# Construindo redes com Servidores

## Informações

- Data: 15/10/2026
- Tema: Construindo redes com Servidores
- Ambiente: Virtual
- Ferramentas: Cisco Packet Tracer

---

## Objetivo

Configurar uma rede utilizando servidores

---

## Topologia

Descreva a estrutura do ambiente.

Exemplo:

PC01 -- PC02 -- PC03 -- PC04 -- PC05 -- PC06   -- SERVIDOR -- SERVIDOR DNS
↓                                                                                              ↓
Switch                                                                                  Switch
↓
Roteador


---

## Equipamentos e Recursos

### Hardware

- NA

### Software

- Cisco Packet Tracer

---

## Configurações Realizadas

### Etapa 1

Foi realizada a distribuição de 6 computadores, switch e roteador  no cisco packet tracer
Após, foi realizada a comunicação dos computadores ao switch e o switch ao roteador.
Após realizar a comunicação via cabo, foi iniciada a configuração logica, partindo primeiramente do roteador para configurar o servidor dhcp.

```bash
COMANDOS UTILIZADOS

# Router(config)#ip dhcp pool fabrica ?
  <cr>
Router(config)#ip dhcp pool fabrica
Router(dhcp-config)#
Router(dhcp-config)#?
  default-router  Default routers
  dns-server      Set name server
  domain-name     Domain name
  exit            Exit from DHCP pool configuration mode
  network         Network number and mask
  no              Negate a command or set its defaults
  option          Raw DHCP option
  network 193.168.3.0 255.255.255.0
  default-router 193.168.3.1
  Router(dhcp-config)#exit
  Router(config)#interface fastEthernet0/0
  Router(config-if)#no shutdown

Router(config-if)#
%LINK-5-CHANGED: Interface FastEthernet0/0, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface
FastEthernet0/0, changed state to up
ip address 193.168.3.1 255.255.255.0
```

### Etapa 2

Aplicar atribuição dhcp em todos os 6 pc´s..

[[2026-10-15 60 Construindo redes com Servidores.jpg]]
![[2026-10-15 60 Construindo redes com Servidores.jpg]]


---
### Etapa 3

Após isso, fizemos a adição de mais um switch e um servidor, onde fizemos a configuração física e manual do mesmo, já que deixamos ele com IP Estático

```bash
COMANDOS UTILIZADOS


enable
configure terminal
interface fastEthernet 0/1
ip address 9.9.9.1 255.0.0.0
no shutdown

````


---


### Etapa 4

Após isso, fizemos a adição de mais um servidor, onde fizemos a configuração física e manual do mesmo, já que deixamos ele com IP Estático, também vamos utilizar esse servidor como servidor DNS

```bash
COMANDOS UTILIZADOS


Router(dhcp-config)#?
  default-router  Default routers
  dns-server      Set name server
  domain-name     Domain name
  exit            Exit from DHCP pool configuration mode
  network         Network number and mask
  no              Negate a command or set its defaults
  option          Raw DHCP options
  dns-server 9.9.9.2
````


---
## Testes Executados

| Teste | Resultado |     |
| ----- | --------- | --- |
| Ping  | OK        |     |
| DHCP  | OK        |     |
| DNS   | OK        |     |

---

## Problemas Encontrados

- NA

---

## Solução Aplicada

- NA

---

## Resultado Final

Foi realizada a comunicação entre as maquinas através da configuração dhcp do roteador que redistribuiu os endereços de ip atraves do switch para cada computador. Tambem foi realizada a configuração de um servidor DNS dentro da rede, e aplicada a configuração no roteador para que possamos resolver nome do site web da Fabrica dentro dela

---

## Lições Aprendidas

- Configurar roteador para funcionar como servidor dhcp
- Como funciona o DHCP
- Configuração de uma rede através do servidor DHCP
- Configuração de um servidor DNS
- Funcionamento do servidor DNS

---

## Evidências

### Prints
![[2026-10-15 60 Construindo redes com Servidores.jpg]]

[[2026-10-15 60 Construindo redes com Servidores 02.jpg]]
![[2026-10-15 60 Construindo redes com Servidores 02.jpg]]

[[2020-10-15 60 Construindo redes com servidores 03.jpg]]
![[2020-10-15 60 Construindo redes com servidores 03.jpg]]

[[2026-10-15 60 Construindo redes com servidores 03.jpg|Open: Pasted image 20261015183759.png]]
![[2026-10-15 60 Construindo redes com servidores 03.jpg]]

### Diagramas

NA

### Arquivos de Configuração
[[35d0a285a487f87cfe5d42b9a102463c_MD5.pkt|Open: 2026-10-15 - Construindo redes com Servidor DHCP.pkt]]
![[35d0a285a487f87cfe5d42b9a102463c_MD5.pkt]]