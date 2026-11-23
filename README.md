<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/capa-dark.png">
  <img src="assets/capa-light.png" width="100%" alt="Nicolas Ponciano e o cubo com os três N">
</picture>

Desenvolvo e mantenho sistemas web corporativos com .NET e SQL Server.

[Meu portfólio](https://nicolasponciano.github.io/) · [LinkedIn](https://www.linkedin.com/in/nicolas-ponciano/)

## Projetos

- **MarcAi** — Criei uma agenda para salões, clínicas e estúdios em que cada profissional tem seus próprios horários. [Experimentar o agendamento](https://marcai-demo.netlify.app/)

  <details>
  <summary>Como trato duas tentativas de reservar o mesmo horário?</summary>

  Calculo os horários disponíveis a partir da agenda do profissional e da duração do serviço. Antes de confirmar a reserva, verifico o conflito no servidor. Uso uma chave de idempotência para reconhecer quando o mesmo pedido chega de novo.

  [![Agenda semanal do MarcAi com atendimentos consecutivos na quinta-feira](assets/agenda.png)](https://nicolasponciano.github.io/assets/projects/marcai/02-agenda.png)

  </details>

- **Seirei** — Fiz um aplicativo que mostra uma tarefa por vez e sincroniza o dia entre o celular e o computador. [Ver as telas do aplicativo](https://nicolasponciano.github.io/#projeto/seirei)

  <details>
  <summary>O que acontece quando a IA não consegue ordenar as tarefas?</summary>

  Guardo no Supabase a ordem em que as tarefas entraram. Quando a IA sugere uma sequência, confiro se ela corresponde às tarefas do dia. Se a chamada falhar, o modo foco segue a ordem de inserção.

  <img src="assets/foco.png" width="520" alt="Tarefa Desenhar a tela de boas-vindas com as opções Concluir e Pular">

  </details>

- **Open Mind** — Escrevi um plugin em TypeScript para consultar minhas notas do Obsidian dentro do OpenCode. [Ler o código do plugin](https://github.com/nicolasponciano/open-mind)

  <details>
  <summary>Como controlo a escrita nas notas do Obsidian?</summary>

  Limitei a leitura à pasta do vault e deixei a escrita desabilitada por padrão. Quando autorizo uma alteração, o plugin compara o hash da nota com o da versão que leu. Assim ele detecta se houve uma edição nesse intervalo.

  </details>

- **ClienteAPI** — Desenvolvi uma API de cadastro de clientes em C# e .NET 8, com dados de contato e endereço no SQL Server. [Ler o código da API](https://github.com/nicolasponciano/ClienteAPI)

  <details>
  <summary>Como uso o CEP no cadastro de clientes?</summary>

  Consulto o ViaCEP para validar o CEP informado e obter os dados do endereço. Salvo o resultado para consultas futuras e uso o CEP também como filtro para encontrar clientes cadastrados.

  </details>
