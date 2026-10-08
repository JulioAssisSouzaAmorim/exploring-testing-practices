# Explorando Práticas de Teste

Neste exercício, vamos explorar práticas de teste em sistemas reais utilizando a ferramenta [TestMiner](https://andrehora.github.io/testminer).

O TestMiner permite visualizar e analisar testes de software em repositórios do GitHub, fornecendo dados sobre como os projetos organizam seus testes, como eles evoluem entre versões e quais bibliotecas de teste são utilizadas.
Explore a ferramenta antes de começar para se familiarizar com seu funcionamento.

Mais detalhes no GitHub da ferramenta: https://github.com/andrehora/testminer.

---

## Passo 1: Selecionar um repositório

Escolha um repositório real que possua testes de software.
Abaixo estão alguns links para ajudá-lo a encontrar projetos interessantes:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

- Tópicos: [ai](https://andrehora.github.io/testminer/#topic:ai), [llm](https://andrehora.github.io/testminer/#topic:llm), [api](https://andrehora.github.io/testminer/#topic:api), [nodejs](https://andrehora.github.io/testminer/#topic:nodejs), [android](https://andrehora.github.io/testminer/#topic:android)

- Por organização: [Google](https://andrehora.github.io/testminer/#google), [Microsoft](https://andrehora.github.io/testminer/#microsoft), [Apple](https://andrehora.github.io/testminer/#apple), [Facebook](https://andrehora.github.io/testminer/#facebook), [Netflix](https://andrehora.github.io/testminer/#netflix), 
[GitHub](https://andrehora.github.io/testminer/#github), [Apache](https://andrehora.github.io/testminer/#apache), [HuggingFace](https://andrehora.github.io/testminer/#huggingface)

## Passo 2: Explorar o repositório selecionado

Busque o repositório escolhido no [TestMiner](https://andrehora.github.io/testminer) e analise os dados de teste gerados pela ferramenta.

## Passo 3: Explicar uma prática de teste

Escolha uma prática ou dado de teste relevante e explique com suas próprias palavras.

---

## Instruções de entrega

1. Faça um `fork` deste repositório (saiba mais sobre forks [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)).
2. Responda às questões abaixo diretamente neste arquivo `README.md` do seu fork. Pode adicionar imagens para enriquecer sua explicação.
3. No Moodle, submeta apenas a URL do seu fork.

---

## Respostas

Repositório: `[<URL_DO_REPOSITÓRIO>](https://github.com/fastapi/fastapi)`

URL TestMiner: `[<URL_NO_TESTMINER>](https://andrehora.github.io/testminer/#fastapi/fastapi)`

Explicação:

**Prática - Code-Driven Development**

No TestMiner, a seção *Test History* nos permite visualizar a evolução no número de testes, helpers e código-fonte geral no repositório da fastapi ao longo de versões consolidadas. Tal acesso nos permite avaliar até que ponto práticas de TDD (Test-Driven Development) foram adotadas no curso do projeto que produziu o programa.

Da release mais antiga até a mais recente, o número de testes explodiu, indo de 4 na versão 0.1.11, para 440 na versão 0.95.2 e 620 na versão 0.143.0. O número de testes CI e helpers cresceu em proporção similar, todos seguindo a tendência geral do código fonte, antes com cardinalidade de 160, e agora (na versão 0.143.0) com cardinalidade de 2199.

Isso nos indica que o número de testes associado ao projeto cresceu significativamente desde sua incepção. Embora parte desse crescimento tenha acompanhando o crescimento do próprio código-fonte, como notamos, é fato que a expansão ainda é um tanto desproporcional, o que é esperado de dinâmicas de desenvolvimento que não fundamentam a criação do código no estabelecimento prévio de testes. Em suma, o programa foi, primeiro, consolidado, e só depois equipado com módulos de teste para validar o trabalho inicial.

Depreende-se daí que a abordagem utilizada, ao menos nas fases iniciais, foi a de Code-Driven Development, uma estratégia mais convencional que a alternativa, Test-Driven Development. A ideia é priorizar a prototipagem rápida e a solução de problemas imediatos pela permissão de desenvolver primeiro para depois validar o que foi desenvolvido. Essa claramente foi a abordagem inicial, mas não se pode extrapolar daí que o projeto não passou a adotar práticas de TDD mais recentemente, o que é perfeitamente praticável, dado o número massivo de testes hoje dispostos.
