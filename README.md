# Explorando Práticas de Teste

Neste exercício, vamos explorar práticas de teste em sistemas reais utilizando a ferramenta [TestMiner](https://andrehora.github.io/testminer).

O TestMiner permite visualizar e analisar testes de software em repositórios do GitHub, fornecendo dados sobre como os projetos organizam seus testes, como eles evoluem entre versões e quais bibliotecas de teste são utilizadas.
Explore a ferramenta antes de começar para se familiarizar com seu funcionamento.

Mais detalhes no GitHub da ferramenta: https://github.com/andrehora/testminer.

---

## Passo 1: Selecionar DOIS repositórios

Escolha dois repositórios reais que possuam testes de software.
Abaixo estão alguns links para ajudá-lo a encontrar projetos interessantes:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

- Tópicos: [ai](https://andrehora.github.io/testminer/#topic:ai), [llm](https://andrehora.github.io/testminer/#topic:llm), [api](https://andrehora.github.io/testminer/#topic:api), [nodejs](https://andrehora.github.io/testminer/#topic:nodejs), [android](https://andrehora.github.io/testminer/#topic:android)

- Por organização: [Google](https://andrehora.github.io/testminer/#google), [Microsoft](https://andrehora.github.io/testminer/#microsoft), [Apple](https://andrehora.github.io/testminer/#apple), [Facebook](https://andrehora.github.io/testminer/#facebook), [Netflix](https://andrehora.github.io/testminer/#netflix), 
[GitHub](https://andrehora.github.io/testminer/#github), [Apache](https://andrehora.github.io/testminer/#apache), [HuggingFace](https://andrehora.github.io/testminer/#huggingface)

## Passo 2: Explorar os repositórios selecionados

Busque os repositórios escolhidos no [TestMiner](https://andrehora.github.io/testminer) e analise os dados de teste gerados pela ferramenta.

## Passo 3: Explicar as prática de teste

Para cada repositório, escolha uma prática ou dado de teste relevante e explique com suas próprias palavras.

---

## Instruções de entrega

1. Faça um `fork` deste repositório (saiba mais sobre forks [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)).
2. Responda às questões abaixo diretamente neste arquivo `README.md` do seu fork. Pode adicionar imagens para enriquecer sua explicação.
3. No Moodle, submeta apenas a URL do seu fork.

---

## Respostas

### Repositório 1 

Repositório: `https://github.com/vercel/ai`

URL TestMiner: `https://andrehora.github.io/testminer/#vercel/ai`

Explicação: Este repositório é um SDK para a construcao de Agentes de IA com Typescript. Escolhi esse repositório para analisar como estão se adaptando as práticas de testes de software para incluir a interacao com LLMs. Pelo que analisei, os testes seguem padrões para mockar os modelos como servicos externos e testam apenas a parte que é garantida pelo SDK, como a preservacao de campos retornados pela API da openAI ('should preserve orchestration usage fields in raw') e garantir que combinacoes de parametros inválidos sejam barrados de serem enviados para a API, e também que os parametros enviados pelo SDK sejam propagados corretamente ao provedor. A prática de teste aqui é condizente com os padroes da industria de mockar servicos externos e realizar o teste apenas com o comportamento que é de propriedade do código a ser testado. Eles utilizam também uma biblioteca de fixtures que contém um repositório de respostas da API da OpenAI para utilizar como base para os mocks. Fontes: (teste unitário 1)[https://github.com/vercel/ai/blob/main/packages/openai/src/responses/openai-responses-language-model.test.ts] e (teste unitário 2)[https://github.com/vercel/ai/blob/main/packages/prodia/src/prodia-image-model.test.ts]

### Repositório 2

Repositório: `<URL_DO_REPOSITÓRIO>`

URL TestMiner: `<URL_NO_TESTMINER>`

Explicação: `<SUA_EXPLICAÇÃO>`
