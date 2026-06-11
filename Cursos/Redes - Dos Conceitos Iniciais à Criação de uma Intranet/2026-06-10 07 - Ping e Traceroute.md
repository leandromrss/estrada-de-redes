---
title: 07 - Ping e Traceroute
allDay: false
startTime: 20:30
endTime: 21:00
date: 2026-06-10
completed: Completeda
---
# Aula


## Conceitos Aprendidos

- Como realizar teste de conectividade utilizando comando "ping" através do CMD
- Como traçar a rota de trafego do pacote enviado pela rede até o destino utilizando o comando "trace route" através do CMD
---

## Anotações
Comandos CMD:

Comando para testar conectividade:
```
-ping + website ou endereço de ip/nome de host do destino
```

Comando para testar conectividade de maneira continua:
```
ping ping + website ou endereço de ip/nome de host do destino -t
```

Comando para traçar rota do pacote:
```
tracert + endereço de destino do pacote
```
O pacote pode variar de rota dependendo do congestionamento da rota. Ela funciona de forma dinâmica, onde o pacote pode alterar a rota caso haja esse congestionamento.

---

## Aplicação Prática

- ping www.youtube.com
- ping www.youtube.com -t
- tracert www.youtube.com

---

## Dúvidas

- Sem duvidas

---

## Status

- [x] Aula concluída
- [x] Revisada
- [x] Consolidada no Resumo Geral

---

## Resumo da Aula

Nessa aula, vemos o conceito de teste de conectividade, onde testamos a nossa conexão com o destino do pacote. Por exemplo, quando tentamos acessar o youtube, podemos utilizar o comando ping através do CMD para verificar se nossa comunicação está funcional com o site.

Também aprendemos a rastrear a rota que o pacote passa através do comando trace route, onde mostra até 30 saltos do caminho que o pacote percorre quando enviamos.