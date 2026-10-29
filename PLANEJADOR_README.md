# AUDI STUDY — Planejador de Estudos

Implementação adicional preservando o `index.html` original (versão de Inglês).

## Funcionalidades
- Cronograma por matéria, tópicos, data da prova, dificuldade e minutos diários.
- Sessões concluídas e progresso armazenados localmente no navegador.
- Exercício guiado de respiração e check-in de preocupação.
- Tutor com respostas locais quando a IA generativa não está configurada.
- Integração **real** com API de IA pelo servidor Node, mantendo a chave fora do navegador.

## Executar
É necessário Node.js 20 ou superior.

```bash
export OPENAI_API_KEY="sua-chave-de-api"
node server.js
```

Abra `http://localhost:3000`.

Sem `OPENAI_API_KEY`, o cronograma continua funcionando e o tutor utiliza orientações locais. Publicar somente `planejador.html` em hospedagem estática **não ativa** a IA generativa; também é necessário hospedar o `server.js` (ou implementar `/api/tutor` em um serviço próprio), configurar a variável de ambiente e providenciar controle de custos, autenticação e política de privacidade antes de uso público com estudantes.

## Arquivos
- `index.html`: projeto anterior, preservado.
- `planejador.html`: novo planejador e interface do tutor.
- `server.js`: servidor e integração com o provedor de IA.

**Importante:** o arquivo local `index(4).html` do Chromebook não foi acessado. Envie esse arquivo ao chat para integrar precisamente o layout e as funções dele.
