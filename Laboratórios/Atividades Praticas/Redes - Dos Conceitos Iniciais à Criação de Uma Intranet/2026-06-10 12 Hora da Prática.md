

## Enunciado da Atividade  
  
Descreva o que foi solicitado pelo instrutor.  
1. Teste a conectividade do seu computador com o servidor que armazena a plataforma da Alura.
2. Verifique as direções que mensagens enviadas do seu computador para a plataforma da Alura seguem.
3. Teste a conectividade do seu computador com a página _[www.utwente.nl](http://www.utwente.nl/)_.
4. Verifique as direções que mensagens enviadas do seu computador para o site _[www.utwente.nl](http://www.utwente.nl/)_ seguem.
5. Analise a diferença nas respostas obtidas.
  
---  
  
## Ambiente Utilizado  
  
- Sistema Operacional:  Windows
- Equipamento:  CMD
- Rede utilizada:  Netwave
  
---  
  
## Procedimento Executado  
  
### Etapa 1  
  
```bash  
ping www.alura.com.br 
```  
  
Foi disparado 4 pacotes de comunicação com o servidor de hospedagem do site da alura, e todos os 4 pacotes retornaram, com um tempo de resposta de 4ms.  
  
---  
  
### Etapa 2  
  
```bash  
Tracert www.alura.com.br  
```  
  
Foram necessários 9 saltos para a rota ser traçada, o tempo médio entre os saltos foi de 4ms. No 7 salto, houve uma latência maior onde o tempo de resposta foi de 32.
  
---  
### Etapa 3 
  
```bash  
ping www.utwente.nl
```  
  
Foi disparado 4 pacotes de comunicação com o servidor de hospedagem do site da utwente, e todos os 4 pacotes retornaram, com um tempo de resposta de 220ms.  
  
---  
  
### Etapa 4  
  
```bash  
Tracert www.utwente.nl  
```  
  
Foram necessários 20 saltos para a rota ser traçada, o tempo médio entre os saltos foi de 220ms. No salto 8, 9 e 11, houve falha em entrega do pacote por uma possível rota congestionada ou distante demais para que a comunicação chegasse antes do timeout.

## Evidências  
  
### Print 1  
  
  [[2026-06-10 12 Evidencia 1.jpg]]
![[2026-06-10 12 Evidencia 1.jpg]]5
  
### Print 2  
  
[[2026-06-10 12 Evidencia 2.jpg]]
![[2026-06-10 12 Evidencia 2.jpg]] 
  
---  
### Print 3  
  
  [[2026-06-10 12 Evidencia 3.jpg]]
![[2026-06-10 12 Evidencia 3.jpg]]

---
### Print 4  
  
[[2026-06-10 12 Evidencia 4.jpg]]
![[2026-06-10 12 Evidencia 4.jpg]]

---
## Resultados Obtidos  
  
Descreva os resultados observados.  
  
Exemplo:  
  
- Ambos os comandos ping retornaram resposta com sucesso
- Comando ping ao servidor da alura teve um tempo médio de resposta de 4ms
- Comando ping ao servidor utwente teve um tempo médio de resposta de 221ms
- Ambos os comandos ping não obtiveram perca de pacotes 
- Comando tracert ao servidor da alura teve um total de 9 saltos, todos concluídos com sucesso e com tempo de resposta médio de 2ms
- Comando tracert ao servidor utwente teve um total de 20 saltos, tendo os saltos: 8, 9 e 11 não completados. Os demais saltos foram concluídos com sucesso e com tempo de resposta médio de 220ms 
  
---  
  
## Análise  
  
  Ambas as rotas retornaram os pacotes e tiveram seus saltos concluídos. A diferença entre os pings e os tracerts realizados, são a latência de comunicação para com ambos os servidores. Possivelmente por estar mais próximo, o servidor da Alura responde de maneira mais rápida e sem perca de pacotes, o que não acontece com o da universidade Twente. Devido a distancia a latência para entrega dos pacotes é muito maior, onde também a perca de pacotes no caminho.
  
---  
  
## Conceitos Aplicados  
  
- ICMP  
- Ping  
- Traceroute  
- Roteamento  
- Latência
  
---  
  
## Dificuldades Encontradas  
  
- Não houve dificuldades encontradas para aplicação e execução da atividade
- Se for considerar uma dificuldade, podemos considerar que a distancia do servidor da universidade Twente implica na velocidade de entrega de pacotes, onde também a perda dos mesmos.
  
---  
  
## Conclusão  
  
Com o conteúdo visitado e estudado, conseguimos realizar a analise de comunicação de um dispositivo a outro dentro da rede. Também conseguimos realizar a analise da rota traçada para essa comunicação e identificar se a mesma está funcional ou com falhas.
  
---  
  
## Aula Relacionada
Essa atividade encerra o primeiro módulo do curso de Redes - Dos Conceitos Iniciais à Criação de Uma Intranet. Sendo assim, estão relacionadas a essa atividade as aulas: 01, 02, 03, 04 e 07. Houve outras aulas que eram atividades dentro da plataforma que verificavam o conteúdo estudado até então, onde não vi necessidade de realizar anotações por se tratar de atividades simples.