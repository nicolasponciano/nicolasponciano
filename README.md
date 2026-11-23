<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/atlas/dark.svg">
  <img src="assets/atlas/light.svg" width="100%" alt="Nicolas Ponciano">
</picture>

**Desenvolvedor de software full stack.** Trabalho com .NET e SQL Server em sistemas web corporativos. Também crio ferramentas para usar no dia a dia e curso pós-graduação em Inteligência Artificial.

[Portfólio](https://nicolasponciano.github.io/) · [LinkedIn](https://www.linkedin.com/in/nicolas-ponciano/)

## Projetos

<a href="#marcai"><img src="assets/atlas/marcai.svg" width="23%" alt="Ir para MarcAi"></a> <a href="#seirei"><img src="assets/atlas/seirei.svg" width="23%" alt="Ir para Seirei"></a> <a href="#open-mind"><img src="assets/atlas/open-mind.svg" width="23%" alt="Ir para Open Mind"></a> <a href="#clienteapi"><img src="assets/atlas/clienteapi.svg" width="23%" alt="Ir para ClienteAPI"></a>

### MarcAi

Criei uma agenda para salões, clínicas e estúdios. A página pública de cada estabelecimento mostra os horários disponíveis por profissional e serviço.

[Experimentar o agendamento](https://marcai-demo.netlify.app/) · <sub>Next.js · TypeScript · PostgreSQL</sub>

<details>
<summary>Como evito duas reservas no mesmo horário?</summary>

Calculo a disponibilidade a partir da agenda e da duração do serviço. Antes de confirmar, verifico o conflito no servidor. Se o mesmo pedido chegar duas vezes, reconheço a repetição pela chave de idempotência.

[![Agenda semanal do MarcAi](assets/agenda.png)](https://nicolasponciano.github.io/assets/projects/marcai/02-agenda.png)

</details>

---

### Seirei

Fiz um aplicativo para trabalhar em uma tarefa por vez e continuar de onde parei ao trocar o computador pelo celular.

[Ver o modo foco](https://nicolasponciano.github.io/#projeto/seirei) · <sub>Next.js · TypeScript · Supabase</sub>

<details>
<summary>E se a IA não conseguir ordenar as tarefas?</summary>

Guardo a ordem de inserção no Supabase. Confiro a sequência sugerida pela IA contra as tarefas do dia e, se a chamada falhar, uso a ordem original.

<img src="assets/foco.png" width="520" alt="Uma tarefa no modo foco, com as opções Concluir e Pular">

</details>

---

### Open Mind

Escrevi um plugin para consultar minhas notas do Obsidian durante uma sessão do OpenCode.

[Explorar o plugin](https://github.com/nicolasponciano/open-mind) · <sub>TypeScript · Node.js · OpenCode</sub>

<details>
<summary>Quando o agente pode alterar uma nota?</summary>

Restrinjo a leitura à pasta do vault e deixo a escrita desabilitada por padrão. Quando autorizo uma alteração, o plugin compara o hash atual com o da versão lida para detectar edições feitas nesse intervalo.

</details>

---

### ClienteAPI

Integrei o ViaCEP a uma API de cadastro de clientes. Posso consultar um endereço pelo CEP e localizar clientes cadastrados na mesma região postal.

[Ler a implementação em C#](https://github.com/nicolasponciano/ClienteAPI) · <sub>C# · .NET 8 · SQL Server</sub>

<details>
<summary>O que acontece depois da consulta ao ViaCEP?</summary>

Salvo os dados do endereço no SQL Server para consultas futuras. A API também permite usar o CEP como filtro ao listar os clientes.

</details>
