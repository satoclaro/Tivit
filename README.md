# Automação de Ligação e WhatsApp — Sistema Tivit / Coop

Aplicação web em HTML/CSS/JavaScript para agilizar o atendimento telefônico e o envio de mensagens formatadas via WhatsApp para o sistema **Tivit / Coop**.

## Funcionalidades

- **Botão de ligação direta no topo:** Aciona `tel:+558007690800` para ligar rapidamente para a Tivit (`+558007690800`).
- **Cola rápida da área de transferência:** Clique em **Nome do cliente**, **Endereço**, **WO** ou **Contrato** para colar automaticamente o conteúdo copiado (com fallback para `Ctrl+V` / colagem manual quando o navegador exigir).
- **Exibição ampliada após formatar:** Ao clicar em **Formatar para WhatsApp** (ou **Formatar e abrir WhatsApp**), exibe em fonte grande:
  - Número no formato `xxx.xxx.xxx`
  - O.S no formato `O.S xxx.xxx.xxxx xxx`
- **Roteiro de fala em tempo real:** Mostra a sequência ordenada dos dados para acompanhamento durante a chamada.
- **Arquivamento, exportação e importação:**
  - **Arquivar chamada:** Salva o registro localmente no navegador (`localStorage`).
  - **Exportar / Importar JSON:** Baixa ou carrega registros em `.json`.
  - **Exportar / Importar CSV:** Baixa ou carrega registros em `.csv`.
- **Baixar em PDF:** Abre a impressão/exportação em PDF formatada para leitura.

## Como usar

1. Extraia o arquivo `.zip` e abra o arquivo `index.html` em qualquer navegador moderno.
2. Use o botão **Ligar Tivit (+55 800 769 0800)** no topo quando necessário.
3. Clique nos campos para colar **Nome do cliente**, **Endereço**, **WO** e **Contrato**.
4. Clique em **Formatar para WhatsApp** para gerar a mensagem, visualizar os números em fonte ampliada e, se desejar, **Arquivar chamada**, **Exportar JSON/CSV**, **Baixar em PDF** ou **Formatar e abrir WhatsApp**.
