# Automação de Ligação e WhatsApp — Sistema Tivit / Coop

Aplicação web em HTML único (`index.html`) para agilizar o atendimento, a ligação e o envio de mensagens formatadas no WhatsApp para o sistema **Tivit / Coop**.

## Funcionalidades

- **Botão de ligação para a Tivit no topo:** aciona diretamente `tel:+558007690800`.
- **Colagem rápida da área de transferência ao clicar:** clique em **Nome do cliente**, **Endereço**, **O.S** ou **Contrato** para colar automaticamente o texto copiado (com fallback para `Ctrl+V` / colar manual caso o navegador exija permissão).
- **Máscaras automáticas:**
  - **Contrato:** `xxx.xxx.xxx`
  - **O.S:** `xxx. xxx.xxx.xxxx`
- **Formatação e envio para WhatsApp:** monta a mensagem na ordem exata do sistema Tivit / Coop, permite copiar ou abrir direto no WhatsApp.
- **Arquivamento de chamadas:** salva o registro da chamada localmente no navegador (`localStorage`) com data/hora, permitindo recarregar nos campos, copiar a mensagem ou excluir.
- **Roteiro de ligação:** exibe os dados na ordem do atendimento em tempo real.

## Como usar

1. Abra o arquivo `index.html` em qualquer navegador moderno (Chrome, Edge, Firefox, Safari).
2. Clique no botão **Ligar Tivit (+558007690800)** no topo quando precisar iniciar a chamada.
3. Copie os dados e clique nos campos correspondentes para colar e formatar automaticamente.
4. Use **Arquivar chamada** para guardar o histórico da chamada no navegador.
