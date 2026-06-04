
# Simulando uma comunicação basica

## Informações

- Data: 03/06/2026
- Tema: Simulação de comunicação de dispositivos de lado A -> B
- Ambiente: Virtual
- Ferramentas: Cisco Packet Tracer

---

## Objetivo

A ideia é entender como funcionaria o envio de uma mensagem disparada por um Smartphone A e o caminho que ela traçaria até chegar ao seu destino que é o smartphone B

---

## Topologia

Descreva a estrutura do ambiente.

Exemplo:

Smartphone A
↓
Roteador
↓
Roteador
↓
Roteador
↓
Roteador
↓
Smartphone B

---

## Equipamentos e Recursos

### Hardware

- Smartphone A
- Smartphone B
- Roteador 0
- Roteador 1
- Roteador 2 
- Roteador 3
- Roteador 4

### Software

- Não utilizado nessa simulação
---

## Configurações Realizadas

### Etapa 1

Descrição da configuração.

```bash
NA
```

### Etapa 2

Descrição da configuração.

```bash
NA
```

---

## Testes Executados

| Teste | Resultado |
| ----- | --------- |
| Ping  | NA        |
| DNS   | NA        |
| DHCP  | NA        |

---

## Problemas Encontrados

- NA
- 

---

## Solução Aplicada

- A simulação acima, mostra um aparelho celular na esquerda (Smartphone0) que dispararia uma mensagem para comunicar com o outro celular (smartphone1) na direita.
	Essa mensagem passaria pelo roteador ao qual o smartphone está conectado, utilizando a camada de aplicação que transportaria essa mensagem por outros roteadores ligados a mesma rede (roteadores do provedor de internet geralmente) através da camada de transporte e rede, que entregaria a mensagem no roteador através da camada física ao qual o smartphone1 está conectado, que faria a entrega dessa mensagem ao smartphone.

---

## Resultado Final

Com essa simulação, podemos entender fisicamente como se dispõe a propagação de comunicação de uma rede A para a rede B e pudemos entender de maneira simples e básica como essas mensagens são enviadas e entregues ao seu destinatário através das camadas de aplicação, transporte, rede e física.

---

## Lições Aprendidas

- Comunicação de Rede A -> Rede B
- Como funciona a camada de Aplicação, Transporte,  Rede e Física.

---

### Prints

[[2026-06-03 04 - Camadas de Rede - Laboratório - Simulando uma comunicação basica.jpg]]
![[2026-06-03 04 - Camadas de Rede - Laboratório - Simulando uma comunicação basica.jpg]]

### Arquivos de Configuração
![[2026-06-03 04 - Camadas de Rede - Laboratório - Simulando uma comunicação basica.pkt]]