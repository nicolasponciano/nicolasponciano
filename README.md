<img align="right" width="34%" src="assets/computador-nicolas.svg" alt="Computador com meu monograma em ciano e lima na tela">

## Olá, sou o Nicolas Ponciano

Desenvolvo sistemas web corporativos com **.NET e SQL Server**. Atualmente curso pós-graduação em Inteligência Artificial.

💻 **Linguagens que uso:** C#, TypeScript e JavaScript.<br>
🛠️ **No dia a dia:** APIs, bancos relacionais e integrações.<br>
✉️ **Onde me encontrar:** [LinkedIn](https://www.linkedin.com/in/nicolas-ponciano/) · [Portfólio](https://nicolasponciano.github.io/)

<br clear="all">

## Meus projetos

<a href="https://marcai-demo.netlify.app/"><img align="left" width="76" height="76" src="assets/projeto-agenda.svg" alt="Abrir MarcAi"></a>

**MarcAi**<br>
Criei uma agenda para salões, clínicas e estúdios. A página pública de cada estabelecimento mostra os horários disponíveis por profissional e serviço.<br>
`Next.js` `TypeScript` `PostgreSQL`<br>
[Experimentar o agendamento](https://marcai-demo.netlify.app/)

<br clear="all">

<details>
<summary>Como evito duas reservas no mesmo horário?</summary>

Calculo a disponibilidade a partir da agenda e da duração do serviço. Antes de confirmar, verifico o conflito no servidor. Se o mesmo pedido chegar duas vezes, reconheço a repetição pela chave de idempotência.

[![Agenda semanal do MarcAi](assets/agenda.png)](https://nicolasponciano.github.io/assets/projects/marcai/02-agenda.png)

</details>

<a href="https://nicolasponciano.github.io/#projeto/seirei"><img align="left" width="76" height="76" src="assets/projeto-foco.svg" alt="Abrir Seirei"></a>

**Seirei**<br>
Fiz um aplicativo para trabalhar em uma tarefa por vez e continuar de onde parei ao trocar o computador pelo celular.<br>
`Next.js` `TypeScript` `Supabase`<br>
[Ver o modo foco](https://nicolasponciano.github.io/#projeto/seirei)

<br clear="all">

<details>
<summary>E se a IA não conseguir ordenar as tarefas?</summary>

Guardo a ordem de inserção no Supabase. Confiro a sequência sugerida pela IA contra as tarefas do dia e, se a chamada falhar, uso a ordem original.

<img src="assets/foco.png" width="520" alt="Uma tarefa no modo foco, com as opções Concluir e Pular">

</details>

<a href="https://github.com/nicolasponciano/open-mind"><img align="left" width="76" height="76" src="assets/projeto-notas.svg" alt="Abrir Open Mind"></a>

**Open Mind**<br>
Escrevi um plugin para consultar minhas notas do Obsidian durante uma sessão do OpenCode.<br>
`TypeScript` `Node.js` `OpenCode`<br>
[Explorar o plugin](https://github.com/nicolasponciano/open-mind)

<br clear="all">

<details>
<summary>Quando o agente pode alterar uma nota?</summary>

Restrinjo a leitura à pasta do vault e deixo a escrita desabilitada por padrão. Quando autorizo uma alteração, o plugin compara o hash atual com o da versão lida para detectar edições feitas nesse intervalo.

</details>

<a href="https://github.com/nicolasponciano/ClienteAPI"><img align="left" width="76" height="76" src="assets/projeto-api.svg" alt="Abrir ClienteAPI"></a>

**ClienteAPI**<br>
Integrei o ViaCEP a uma API de cadastro de clientes. Posso consultar um endereço pelo CEP e localizar clientes cadastrados na mesma região postal.<br>
`C#` `.NET 8` `SQL Server`<br>
[Ler a implementação em C#](https://github.com/nicolasponciano/ClienteAPI)

<br clear="all">

<details>
<summary>O que acontece depois da consulta ao ViaCEP?</summary>

Salvo os dados do endereço no SQL Server para consultas futuras. A API também permite usar o CEP como filtro ao listar os clientes.

</details>
