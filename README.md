<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/logo-dark.svg">
  <img align="right" width="88" alt="Monograma de Nicolas Ponciano" src="assets/logo-light.svg">
</picture>

# Nicolas Ponciano

**Desenvolvedor de software full stack**

Desenvolvo sistemas web corporativos com **.NET e SQL Server**. Também crio ferramentas para o meu dia a dia e curso pós-graduação em Inteligência Artificial.

[Meu portfólio](https://nicolasponciano.github.io/) · [LinkedIn](https://www.linkedin.com/in/nicolas-ponciano/)

<br clear="all">

## Projetos


<img align="left" width="52" height="52" alt="" src="assets/projeto-agenda.svg">

### MarcAi

<sub>Next.js · TypeScript · PostgreSQL</sub>

Criei uma agenda para salões, clínicas e estúdios. Quem vai marcar um horário escolhe o serviço e vê a disponibilidade do profissional.

[Experimentar o agendamento](https://marcai-demo.netlify.app/)

<details>
<summary>Como trato duas tentativas de reservar o mesmo horário?</summary>

Calculo os horários disponíveis a partir da agenda do profissional e da duração do serviço. Antes de confirmar a reserva, verifico o conflito no servidor. Uso uma chave de idempotência para reconhecer quando o mesmo pedido chega de novo.

[![Agenda semanal do MarcAi com atendimentos consecutivos na quinta-feira](assets/agenda.png)](https://nicolasponciano.github.io/assets/projects/marcai/02-agenda.png)

</details>

<img align="left" width="52" height="52" alt="" src="assets/projeto-foco.svg">

### Seirei

<sub>Next.js · TypeScript · Supabase</sub>

Fiz um aplicativo que mostra uma tarefa por vez e mantém a lista sincronizada entre o celular e o computador.

[Conhecer o modo foco no portfólio](https://nicolasponciano.github.io/#projeto/seirei)

<details>
<summary>O que acontece quando a IA não consegue ordenar as tarefas?</summary>

Guardo no Supabase a ordem em que as tarefas entraram. Quando a IA sugere uma sequência, confiro se ela corresponde às tarefas do dia. Se a chamada falhar, o modo foco segue a ordem de inserção.

<img src="assets/foco.png" width="520" alt="Tarefa Desenhar a tela de boas-vindas com as opções Concluir e Pular">

</details>

<img align="left" width="52" height="52" alt="" src="assets/projeto-notas.svg">

### Open Mind

<sub>TypeScript · Node.js · OpenCode</sub>

Escrevi um plugin em TypeScript para consultar minhas notas do Obsidian dentro do OpenCode.

[Explorar o plugin para OpenCode](https://github.com/nicolasponciano/open-mind)

<details>
<summary>Como controlo a escrita nas notas do Obsidian?</summary>

Limitei a leitura à pasta do vault e deixei a escrita desabilitada por padrão. Quando autorizo uma alteração, o plugin compara o hash da nota com o da versão que leu. Assim ele detecta se houve uma edição nesse intervalo.

</details>

<img align="left" width="52" height="52" alt="" src="assets/projeto-api.svg">

### ClienteAPI

<sub>C# · .NET 8 · SQL Server</sub>

Integrei o ViaCEP a uma API em C# e .NET 8 para cadastrar clientes e buscar endereços por CEP. Uso SQL Server para guardar os dados.

[Ver a implementação em C#](https://github.com/nicolasponciano/ClienteAPI)

<details>
<summary>Como uso o CEP no cadastro de clientes?</summary>

Consulto o ViaCEP para validar o CEP informado e obter os dados do endereço. Salvo o resultado para consultas futuras e uso o CEP também como filtro para encontrar clientes cadastrados.

</details>
