<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/editorial-dark.svg">
  <img src="assets/editorial-light.svg" width="100%" alt="Nicolas Ponciano — Desenvolvimento de software">
</picture>

Desenvolvo sistemas web corporativos com **.NET e SQL Server**. Também escrevo ferramentas que uso no dia a dia e curso pós-graduação em Inteligência Artificial.

[Visitar meu portfólio](https://nicolasponciano.github.io/) · [Conversar no LinkedIn](https://www.linkedin.com/in/nicolas-ponciano/)

## Projetos

| Projeto | O que construí |
| :--- | :--- |
| **MarcAi** | Criei uma agenda por profissional para salões, clínicas e estúdios. [Experimentar a demo](https://marcai-demo.netlify.app/) |
| **Seirei** | Fiz um aplicativo que mostra uma tarefa por vez e sincroniza o dia entre dispositivos. [Ver o modo foco](https://nicolasponciano.github.io/#projeto/seirei) |
| **Open Mind** | Escrevi um plugin para consultar minhas notas do Obsidian dentro do OpenCode. [Explorar o plugin](https://github.com/nicolasponciano/open-mind) |
| **ClienteAPI** | Integrei o cadastro de clientes ao ViaCEP em uma API com C# e .NET 8. [Ler o código](https://github.com/nicolasponciano/ClienteAPI) |

## Decisões de implementação

<details>
<summary><strong>MarcAi</strong> · Como trato duas tentativas de reservar o mesmo horÃ¡rio?</summary>

<sub>Next.js · TypeScript · PostgreSQL</sub>

Calculo os horÃ¡rios disponÃ­veis a partir da agenda do profissional e da duraÃ§Ã£o do serviÃ§o. Antes de confirmar a reserva, verifico o conflito no servidor. Uso uma chave de idempotÃªncia para reconhecer quando o mesmo pedido chega de novo.

[![Agenda semanal do MarcAi com atendimentos consecutivos na quinta-feira](assets/agenda.png)](https://nicolasponciano.github.io/assets/projects/marcai/02-agenda.png)

</details>

<details>
<summary><strong>Seirei</strong> · O que acontece quando a IA nÃ£o consegue ordenar as tarefas?</summary>

<sub>Next.js · TypeScript · Supabase</sub>

Guardo no Supabase a ordem em que as tarefas entraram. Quando a IA sugere uma sequÃªncia, confiro se ela corresponde Ã s tarefas do dia. Se a chamada falhar, o modo foco segue a ordem de inserÃ§Ã£o.

<img src="assets/foco.png" width="520" alt="Tarefa Desenhar a tela de boas-vindas com as opÃ§Ãµes Concluir e Pular">

</details>

<details>
<summary><strong>Open Mind</strong> · Como controlo a escrita nas notas do Obsidian?</summary>

<sub>TypeScript · Node.js · OpenCode</sub>

Limitei a leitura Ã  pasta do vault e deixei a escrita desabilitada por padrÃ£o. Quando autorizo uma alteraÃ§Ã£o, o plugin compara o hash da nota com o da versÃ£o que leu. Assim ele detecta se houve uma ediÃ§Ã£o nesse intervalo.

</details>

<details>
<summary><strong>ClienteAPI</strong> · Como uso o CEP no cadastro de clientes?</summary>

<sub>C# · .NET 8 · SQL Server</sub>

Consulto o ViaCEP para validar o CEP informado e obter os dados do endereÃ§o. Salvo o resultado para consultas futuras e uso o CEP tambÃ©m como filtro para encontrar clientes cadastrados.

</details>
