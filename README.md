# DIO Agent na Prática

Desafio de Projeto da [DIO](https://dio.me): configure o [DIO Agent](https://github.com/digitalinnovationone/dio-agent) e use as skills dele para estudar, praticar e planejar a sua carreira.

----

## 1. Configure o DIO Agent
Oi!
Quem é você e como pode me ajudar nos meus estudos na DIO?

Eu sou o **DIO Agent**, um mentor de tecnologia criado para acompanhar estudantes da DIO na jornada de aprendizado. Minha missão não é te entregar respostas prontas, mas te ajudar a ganhar autonomia e confiança para resolver problemas sozinho e se preparar para o mercado.

Na prática, posso te ajudar de quatro formas principais:

- **Montar um plano de estudos:** organizamos o que estudar, em que ordem e no ritmo da sua rotina, conectando com experiências da DIO (como Bootcamps, Formações, Cursos, Acelerações ou English4Tech).
- **Explicar conceitos e tecnologias:** tiro dúvidas sobre programação, ferramentas ou termos técnicos de um jeito simples, usando exemplos práticos.
- **Destravar desafios:** se você travar em um Desafio de Código, de Projeto ou Criativo, eu te guio com dicas graduais para você chegar na solução sem pular o aprendizado.
- **Tirar dúvidas sobre o mercado e atualidades:** posso buscar informações atualizadas sobre tecnologias, versões e novidades da área.

  ----

## 2. Estudar

Me explica o que é uma skill de um agente de IA.
Meu nível: uso IA no dia a dia, mas nunca configurei um agente.

Perfeito! Como você já usa IA no dia a dia, vai ficar bem fácil de visualizar.

O que é uma Skill?

 Uma Skill (habilidade) é um guia passo a passo focado em uma tarefa específica que você deixa disponível para um agente de IA. Em vez de você ter que digitar um prompt gigante toda vez que quer o mesmo tipo de resultado, a Skill ensina ao agente quando usar aquele guia e como executar a tarefa do jeito certo.

(Só para alinhar o termo: um agente de IA é uma IA que não apenas conversa, mas também consegue seguir rotinas e usar ferramentas para executar tarefas por conta própria.)

Uma analogia do dia a dia

Pense em um chef de cozinha (o agente de IA). Ele já sabe cozinhar de forma geral. Mas, se você quer que um prato específico saia sempre no padrão da casa, você entrega a ele uma ficha de receita (a Skill).

Ele não precisa segurar todas as receitas na cabeça o tempo todo: só pega a ficha daquele prato na hora em que o pedido chega e segue os passos certinho.

Exemplo prático
Na prática, muitas Skills são apenas arquivos de texto simples (geralmente em Markdown, que é um formato de texto com títulos e listas). Imagine uma Skill para resumir aulas:
name: resumir-aula
description: Use quando o estudante pedir para resumir uma aula ou anotação.

# Como resumir uma aula

1. Destaque os 3 pontos principais em tópicos curtos.
2. Explique cada termo técnico novo em 1 frase.
3. Termine com 2 perguntas rápidas para revisar o conteúdo.

Com isso configurado, toda vez que você pedir "resume essa aula pra mim", o agente reconhece a descrição, abre essa Skill e segue exatamente esse formato — sem você precisar repetir as instruções.

Um engano comum

Muita gente confunde Skill com ferramenta (ou acha que precisa saber programar código complexo para criar uma). A diferença é simples:

Ferramenta é o recurso que o agente usa (como pesquisar na web ou ler um arquivo) — tipo o fogão e as panelas.
Skill é o método de trabalho (o passo a passo em texto) — tipo a receita.

-----

## 3. Praticar

Estou travado em um Desafio de Código da DIO.
O desafio pede a soma de todos os números de 1 até N.
Meu código imprime só o último número, não a soma:
let n = parseInt(gets());
let soma = 0;
for (let i = 1; i <= n; i++) {
  soma = i;
}
print(soma);
Me ajuda a destravar sem dar a resposta pronta.

Você está **muito** perto! A estrutura do seu código já está certinha: você leu a entrada com `gets()`, começou `soma` em `0`, montou o laço `for` de `1` até `n` e exibiu o resultado com `print(soma)`.

O ponto para olhar está bem aqui dentro do laço:
```js
soma = i;
```

### O conceito por trás do erro
Quando usamos o operador `=`, estamos **substituindo** o valor que estava guardado na variável por um novo. Pense no que acontece se `n` for `3`:
- Na 1ª volta (`i = 1`): `soma` vira `1`.
- Na 2ª volta (`i = 2`): `soma` vira `2` (o `1` anterior é apagado!).
- Na 3ª volta (`i = 3`): `soma` vira `3` (e é só isso que aparece no final).

Para somar de 1 até `n`, a variável `soma` precisa funcionar como um **acumulador** — ou seja, guardar o que ela já tinha **junto** com o novo número `i`.

Olhando para essa linha `soma = i;`, como você mudaria o lado direito do `=` para aproveitar o valor que já estava guardado em `soma` em vez de apagá-lo?

-------

## 4. Planejar

Quero montar um plano de estudos.
Trilha: Formação IA Builder
Objetivo: concluir em 02 meses
Meu nível: iniciante
Tempo: 01  hora por dia, de segunda a sexta feira

### Aqui está um plano de estudos realista de **2 meses (8 semanas)**, pensado para caber na sua rotina sem correria.

-----

### Resumo do seu plano
- **Base na DIO:** Carreira **AI Builder** ([dio.me/#careers](https://www.dio.me/#careers)), começando pelo seu bootcamp atual (**IA na Prática**) e avançando para as formações iniciais da trilha.
- **Perfil:** iniciante (já fazendo *IA na Prática* e dando os primeiros passos em Python).
- **Ritmo:** 1 hora por dia, de segunda a sexta (**5h por semana**, totalizando cerca de **40 horas estimadas** em 8 semanas).

> *Nota sobre o tempo:* como a carga horária exata varia conforme a formação que você escolher abrir na plataforma, a divisão abaixo é uma **estimativa** baseada nas formações principais da trilha AI Builder na DIO. Se você já estiver com uma Formação específica aberta e quiser que eu detalhe **módulo por módulo**, é só colar o link ou os títulos dos módulos aqui!

----

### Como organizar sua 1 hora diária
- **Segunda a Quinta (1h/dia):** 35–40 min de aula + 20–25 min praticando na hora (testando prompts, ferramentas ou pequenos ajustes no seu projeto).
- **Sexta-feira (1h):** revisão leve da semana + foco nos **Desafios** (de Projeto ou Criativos) para ir alimentando o seu GitHub.

---

### Cronograma de 8 semanas

#### Semanas 1 e 2 (10h) — Base sólida: *Inteligência Artificial na Prática*
- **Foco:** concluir o bootcamp que você já está fazendo — entender como funcionam os modelos de IA, estruturar bons prompts, dar contexto e trabalhar com assistentes/agentes (como o DIO Agent).
- **Prática:** finalizar os desafios pendentes do bootcamp (incluindo o seu README no GitHub).
- **Marco da Semana 2:** Bootcamp *IA na Prática* concluído e publicado no seu portfólio.

#### Semanas 3, 4 e 5 (15h) — Construindo apps reais: *Formação AI Builder com Lovable*
- **Foco:** aplicar o ciclo de AI Builder (**pedir, conferir e construir**) para tirar MVPs do papel rapidamente usando IA.
- **Prática:** essa formação trabalha criação de aplicativos práticos — inclusive dá para conectar direto com a sua ideia do **app de finanças pessoais com educador financeiro**!
- **Marco da Semana 5:** primeiro MVP funcional rodando e documentado no GitHub.

#### Semanas 6 e 7 (10h) — IA no dia a dia: *Formação IA Aplicada a Negócios*
- **Foco:** usar ferramentas de IA para resolver problemas reais e otimizar rotinas e processos.
- **Prática:** aplicar o que aprender para deixar seu projeto mais útil no dia a dia (como automatizar registros ou gerar resumos financeiros).
- **Marco da Semana 7:** pelo menos uma rotina ou melhoria com IA funcionando de ponta a ponta.

#### Semana 8 (5h) — Consolidação e Portfólio
- **Foco:** revisar os projetos feitos nos 2 meses, melhorar os READMEs no GitHub e participar de uma **Live ou Mentoria** da DIO para tirar dúvidas sobre o mercado de AI Builder.
- **Próximos passos (após os 2 meses):** quando estiver mais confortável — inclusive com o Python que você está estudando —, você pode seguir para as formações mais técnicas da carreira, como *Desenvolvimento de SaaS com IA e Claude Code* ou *Orquestração Avançada de Agentes de IA*.
- **Marco da Semana 8:** portfólio com seus primeiros projetos de AI Builder no ar e clareza do próximo degrau.

---

### Dica para manter a constância
Na plataforma da DIO, dentro dos Bootcamps e Formações em que você está inscrita, vale registrar essa rotina de **1h por dia (segunda a sexta)** na ferramenta **Meta de Estudo**. Ela te ajuda a acompanhar seu avanço e envia lembretes por e-mail para não perder o ritmo.

*(E ao longo dessas 8 semanas, sempre que travar em um desafio ou conceito novo, é só trazer para cá que a gente destrava juntas!)*

Esse ritmo de 8 semanas parece realista para a sua rotina, ou você prefere ajustar alguma parte (ou detalhar os módulos exatos de alguma formação específica)?

-----

 Bônus: seu próximo passo

Se você quer construir com IA:

Quero escolher meu próximo passo na Carreira AI Builder.
Quero construir: Um APP para controle de finanças pessoais, com educador financeiro
Programação: básico, comecei linguagem em Python agora
Objetivo: tirar uma ideia do papel

-------

### Para o seu momento — **tirar do papel um app de finanças pessoais com educador financeiro estando no início do Python** — o melhor próximo passo na **Carreira AI Builder** da [DIO](https://dio.me) é seguir para a **Formação AI Builder com Lovable**.

### Por que esse é o melhor passo agora?
- **Tira a ideia do papel sem travar no código:** em vez de esperar meses para dominar programação web completa, você usa **Vibe Coding** (construir aplicativos orientando a IA com instruções claras em linguagem natural) para criar um **MVP** real e utilizável bem mais rápido.
- **Alinhado 100% ao seu projeto:** o foco é transformar ideias em apps funcionais do dia a dia — exatamente o cenário do seu gerenciador de finanças com receitas, as 6 categorias de gastos e o educador financeiro.
- **Respeita sua fase atual:** você já coloca seu app para rodar enquanto continua construindo sua base de **Python** e **SQL** em paralelo nas férias da faculdade de Ciências de Dados.

### Como ficam os passos seguintes na sua evolução
1. **Agora (fechar a base):** concluir o bootcamp **IA na Prática** e entregar seu desafio no GitHub.
2. **Próximo passo imediato:** **Formação AI Builder com Lovable** → tirar o MVP do seu app de finanças do papel.
3. **Depois (ampliar automações):** **Formação Inteligência Artificial Aplicada a Negócios** → conectar fluxos e automações práticas ao seu dia a dia.
4. **Mais adiante (nível técnico avançado):** quando já estiver mais confortável programando, partir para **Desenvolvimento de SaaS com IA e Claude Code** ou **Orquestração Avançada de Agentes de IA** para deixar seu educador financeiro ainda mais inteligente e personalizado.

E o melhor: com o seu **DIO Global vitalício**, toda essa escadinha já está disponível para você evoluir no seu ritmo!

-----

### Como foi para você

 Muito interessante, várias ideias na cabeça para usufruir bem desse agente. Me aguardem!!!
