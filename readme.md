# Teste de Performance com JMeter 

Projeto de teste de performance utilizando JMeter e plugins na API e página Web de uma loja virtual simulada para testes, elaborada pelo Professor Júlio de Lima.

> **Apache Jmeter** é uma ferramenta Java puro de código aberto projetada para testar o desempenho de aplicativos e servidores web, medir a capacidade de carga e analisar o desempenho em diferentes cenários. Ele é amplamente utilizado para realizar testes de carga, testes de estresse, testes de desempenho, e outros tipos de testes de software.

<img src= "assets/Apache_JMeter" height=100 width=100/>
<img src = "assets/quality-assurance" height=100 width=100/>

## Conceito de Teste de Performance 

Determinando como o sistema se comporta em termos de velocidade, capacidade de resposta, escalabilidade e estabilidade.

## Estratégias de Teste de Performance

Geralmente giram em torno de 5 atributos chave, onde devemos começar a perguntar antes das estratégias: 
**O objetivo, a quantidade de usuários, o tempo de uso, o cenário a ser executado e o resultado esperado.**
Os **testes** mais comuns são:
-   Desempenho
-   Carga
-   Estresse

> Nesse projeto iremos utilizar estratégias de **Desempenho**

## Planejando o Teste de Desempenho

 - [ ] Objetivo: Validar o bom funcionamento com múltiplos usuários acessando o aplicativo ao mesmo tempo
 - [ ] Quantidade de Usuários: 50 usuários simultâneos
 - [ ] Tempo de Execução: N/A
 - [ ] Cenário: Cadastro de Produto
 - [ ]  Resultado Esperado: Tempo de carregamento máximo de 3 segundos

> 
## Data Driven Test

Através do “Configuração dos dados CSV” utilizamos a massa de dados para simular 5 usuários simultâneos cadastrando produtos em média de 5 segundos.

## Algumas das Métricas Avaliadas
-   Mínimo e Máximo:
    -   Menor e maior tempo dentre toda a população de requisições que foram exercitadas.
-   Média e Desvio Padrão
    -   O valor médio e seu desvio para demonstrar a distribuição do valor médio da população.
-   Percentil de 90 (Linha dos 90) e a Mediana
    -   O valor máximo obtido para um percentual da população que contribua para a tomada de decisão. ( “90% dos nossos usuários tem um tempo máximo de resposta de 200ms” )

---
Apache JMeter
 https://jmeter.apache.org/
 
Plugins de métricas de teste
https://jmeter-plugins.org/wiki/PluginsManager/
