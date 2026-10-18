<div align="center">

# Learnix

**Um tutor de IA que monta o material de estudo, guarda suas notas e cobra o que você errou.**

Feito para estudantes brasileiros que se preparam para o ENEM · Em desenvolvimento · [Prévia →](https://learnix.bulga.top)

[English](README.md) · [Visão do produto](docs/product.md) · [Como é construído](docs/architecture.md)

</div>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.jpg">
  <img alt="O espaço de estudo do Learnix: notas, tutor e editor lado a lado" src="assets/hero-light.jpg">
</picture>

> **Sobre este repositório.** O Learnix é um SaaS comercial em desenvolvimento, então o código-fonte é privado. Este repositório é a vitrine pública: o que o produto faz, como foi projetado e o que eu construí. Se quiser uma demonstração ou algo parecido feito para você, veja [Trabalhe comigo](#trabalhe-comigo).

## O que faz

A maioria das ferramentas de estudo é um chatbot que esquece tudo ou um banco de questões que ignora o que você já sabe. O Learnix mantém **um espaço por tema** e liga as duas coisas:

1. **Crie um estudo** sobre qualquer tema ("Funções logarítmicas para o ENEM").
2. **Converse com o tutor.** Ele monta o material aos poucos: visão geral, um conceito por vez, exemplos resolvidos e fórmulas renderizadas. Com a pesquisa na web ligada, cita as fontes.
3. **Guarde o que importa.** As respostas viram notas em Markdown, com histórico de versões e ramificações. Todo estudo também tem um mapa mental editável e flashcards.
4. **Pratique.** As questões são geradas para o tema, em modo **treino** (correção a cada questão) ou **simulado** (cronometrado, correção no final). Você informa a confiança em cada resposta, e o resultado separa *domínio* de *chute*.
5. **Revise os erros.** As questões erradas voltam como foco da próxima rodada.

Há ainda uma demonstração sem conta, provas avulsas que se adaptam às suas tentativas anteriores, sequência de estudo, flashcards com repetição espaçada e um ranking opcional.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/questao-dark.jpg">
  <img alt="Questão no estilo ENEM corrigida, com explicação" src="assets/questao-light.jpg" width="640">
</picture>

## Destaques de engenharia

O trabalho interessante está em tornar os recursos de IA confiáveis e baratos o bastante para vender. Mais detalhes (em inglês) em [docs/architecture.md](docs/architecture.md).

| Problema | O que construí |
| --- | --- |
| Respostas longas de IA se perdem ao recarregar ou reiniciar | Cada resposta do tutor é um **trabalho durável** no banco; a exibição ao vivo é um fluxo de eventos separado, que pode ser retomado ou substituído por consulta periódica. |
| Questões escritas por IA costumam ser ambíguas ou erradas | **Pesquisa** (com cache por tema), **autoria com esquema estrito** e **revisão cega**: o revisor responde sem ver o gabarito, e divergências reescrevem só aquela questão. |
| O custo da IA pode passar do valor da assinatura | O uso é medido pelo **custo real** contra um orçamento mensal por plano. |
| Testar não deveria exigir cadastro | **Demonstração sem custo**, convertida em conta real sem perder nada. |

## Tecnologias

`Go` · `chi` · `templ` · `htmx` · `Alpine.js` · `Tailwind CSS` · `KaTeX` · `SQLite` · `Stripe` · LLMs por API compatível com OpenAI · pesquisa na web com citações

## Trabalhe comigo

Construo produtos completos com foco em backend: APIs, modelagem de dados, recursos de IA com controle de custo, cobrança e uma interface cuidada.

- Portfólio: [bulgaaw.com/pt](https://bulgaaw.com/pt/)
- E-mail: [me@bulgaaw.com](mailto:me@bulgaaw.com)
- X: [@LinkyDevv](https://x.com/LinkyDevv)
- GitHub: [bulgadev](https://github.com/bulgadev)

## Licença

Todos os direitos reservados. O código-fonte é privado. O texto e as imagens deste repositório não podem ser reutilizados sem permissão.
