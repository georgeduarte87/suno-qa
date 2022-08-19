# Desafio QA

## Objetivo
A proposta deste desafio é analisar as suas habilidades em conceber cenários de testes, design, programação e boas práticas necessárias para automatização dos testes.
Vamos considerar e avaliar todas etapas, caso tenha dúvidas referentes ao Desafio, sinta-se a vontade para entrar em contato com nosso time.

### 1. Etapa (Frontend)

Nessa etapa é necessário elaborar um relatório contendo os principais problemas encontrados. É importante que o relatório seja organizado e de fácil compreensão.

* Conferir layout esperado no [Figma](https://www.figma.com/file/aSgLsRxNxQHzUQLH6yP8nR/Teste-QA?node-id=0%3A1).
* Conferir projeto desenvolvido em `desafio-frontend` clicando [aqui](https://gitlab.com/suno-public/desafio-qa/-/tree/main).

> #
> ##### Para acessar o relatório gerado, [clique aqui](https://github.com/georgeduarte87/suno-qa/blob/main/Relatorio-de-validacao-Front-end.pdf).
>
> ###### Processo realizado: 
> - 15/08:
>   - 1:00 Leitura das instruções e reconhecimento do material enviado para avaliação e organização das ideias para o relatório. 
>   - 2:00 Início do apontamento das divergêncoias encontradas em relação ao layout proposto e o aplicado, finalizando a inspeção do menu e da aba de perfil.
> - 16/08:
>   - 2:00 Finalização do levantamento das inconsistências e geração do relatório para avaliação.
> #

---
### 2. Etapa (Backend)

Você deve criar uma suite de testes (automatizada ou não) com a [API](https://www.themoviedb.org/)

* Foque em cenários críticos.
* Em seu README, detalhar como realizar as configurações necessárias para rodar o projeto em nossa máquina local.

> #
> ###### Metodologia:
> - 16/08:
>   - 1:00 Acessei a documentação da api, disponível [aqui](https://developers.themoviedb.org/3/getting-started/introduction) e realizei uma leitura para entendimento da aplicação e da organização da mesma.
>   - 1:00 Importei a documentação da API usando este [link](https://api.stoplight.io/v1/versions/9WaNJfGpnnQ76opqe/export/oas.json) para o [Postman](https://www.postman.com/) e iniciei a realizar chamadas exploratórias para realizar um reconhecimento das chamadas e explorar os cenários possíveis.
>   - 1:00 Configurei a autenticação da API, e iniciei a salvar os valores em variáveis para realizar os testes exploratórios gerais e obter todo o spectro das 140 rotas disponíveis na API, para organizar e priorizar cenários.
> - 17/08:
>   - 3:00 Finalizei a configuração de todas as chamadas com todas as variáveis e um teste básico de status code, para já poder estar monitorando ao menos o resultado das rotas.
>   - 1:00 Instalei [Newman](https://www.npmjs.com/package/newman) na máquina local e organizei os cenários de testes para poder executar de forma automatizada e independente.
>   - 1:00 Subi o Relatório de testes e a coleção de testes exploratórios da API para o reposítório, organizei as informações e o processo utilizado no desenvolvimento no reposítório e configurei o pipeline do repositório no Github Actions para executar os testes criados utilizando o Newman a cada atualização do repositório.
> - 18/08:
>   - 1:00 Detalhei o processo utilizado até aqui, descrevento as etapas e planejei a organização e os próximos passos, priorizando cenários mais críticos para a realização de testes mais específicos.
>   - 3:00 Trabalhei na automação dos cenários escolhidos.
>   - 1:00 Finalizei e revisei os cenários, subi as alterações para o repositório, revisei os detalhes da entrega do repositório e escrevi o email de entrega do desafio.
>
> Para executar os testes, basta importar as duas coleções `TesteAPI.json` e `TesteAPICriticos.json` 
> Também é possível executar as coleções utiizando newmanjs, para isso será necessário instalar NodeJs e o pacote do Newman mencionado acima e executar o comando `newman run .\TesteAPICriticos.json --delay-request 100` e `newman run .\TesteAPI.json --delay-request 100`.
> #


### 3. Processo de submissão e prazo de entrega

1. É necessário ter um repositório no GitLab/GitHub para hospedar o projeto.
2. O repositório deverá ser público.
3. Prazo de entrega de 5 dias úteis.
4. Encaminhar o link do repositório e os documentos do teste técnico por email (desafiosti@suno.com.br).


### 4. Considerações finais

Para realiazação dos testes, você pode escolher a linguagem de programação, framework, etc. que você se sentir mais confortável.
Não se esqueça de prover informações detalhadas de como instalar e rodar as suítes de teste.
Vamos considerar e avaliar todas etapas.


#### Metodologia: 
Para acessar a documentação da API utilizada como base, clique [aqui](https://developers.themoviedb.org/3/getting-started/introduction).

...

https://api.stoplight.io/v1/versions/9WaNJfGpnnQ76opqe/export/oas.json