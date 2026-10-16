
# Construindo redes com Roteadores

## Informações

- Data: 15/10/2026
- Tema: Construindo redes com roteadores
- Ambiente: Virtual
- Ferramentas: Cisco Packet Tracer

---

## Objetivo

Configurar uma rede utilizando roteadores

---

## Topologia

Descreva a estrutura do ambiente.

Exemplo:

PC01 -- PC02 -- PC03
↓
roteador



---

## Equipamentos e Recursos

NA

### Hardware

- NA 

### Software

- Cisco Packet Tracer

---

## Configurações Realizadas

### Etapa 1

Foi realizada a configuração do roteador utilizando seu próprio painel de configuração utilizando os seguintes comandos:

```bash
# interface (nome da porta) para acessar a configuração da porta especificicada
# no shutdown (para mante-la ligada e ativa)
# interface (nome da porta) para acessar a configuração da porta especificicada
# ip address + ip e mascara de subrede para definição de ip da porta
# exit (para sair da configuração da porta)
# show ip interface + (nome da interface) para verificar o endereço de ip da porta
```

### Etapa 2

Foi atribuído o IP para cada computador conforme configurado em cada porta e também configurado o gateway em cada maquina dentro da rede

---

## Testes Executados

| Teste | Resultado |
| ----- | --------- |
| Ping  | OK        |
|       |           |
|       |           |

---

## Problemas Encontrados

- NA


---

## Solução Aplicada

- NA

---

## Resultado Final

Foi realizada a comunicação entre as maquinas através do teste ping

---

## Lições Aprendidas

- Configuração de varias subredes dentro de um roteador
- Comunicação de uma maquina de diferentes endereços de rede

---

## Evidências

### Prints

[[2026-10-15 41 Construindo redes com Roteadores.jpg]]
![[2026-10-15 41 Construindo redes com Roteadores.jpg]]

### Diagramas
NA

### Arquivos de Configuração!
[[2026-10-15 - Construindo redes com Roteadores.pkt]]