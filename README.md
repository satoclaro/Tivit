# Roteiro de Chamada — Sistema Tivit / Coop

Aplicação web local (`index.html`) desenvolvida para agilizar o atendimento e o registro de chamadas técnicas no sistema **Tivit / Coop**.

## Funcionalidades

- **Botão de Ligação Rápida no Topo:** Discagem direta para `+558007690800` via link `tel:+558007690800`.
- **Colagem Automática ao Clicar:** Clicar nos campos **Nome do Cliente**, **Endereço**, **WO / O.S.** ou **Contrato** lê o conteúdo da área de transferência e preenche o campo automaticamente (com suporte a digitação e `Ctrl+V` caso o navegador exija permissão).
- **Máscaras de Formatação:**
  - **Contrato:** `xxx.xxx.xxx`
  - **WO / O.S.:** `xxx.xxx.xxx.xxxx`
- **Botão Limpar Campo Opção:** Localizado logo abaixo do campo **Opção / Observação Adicional** para limpar rapidamente caso haja cópia ou digitação incorreta.
- **Ordem Fixa de Parâmetros:** Mantém na sequência definida:
  - `Opção do serviço: 239`
  - `Cidade: 003`
  - `Código da empresa: 68804663#`
  - `Nome do Funcionário: Fernando Sato`
  - `Código Funcionário: Z688632`
  - `Nome da Conveniada: CSR Engenharia Ltda`
  - `PDA: 91520-6585`
  - `Código da Baixa: 409`
  - `Tipo de wo: Instalação/ Mudança de Pacote`
  - `Hora de Início : 12:00`
- **Formatação para WhatsApp:** Gera a mensagem formatada com negrito e marcadores pronta para envio no WhatsApp.
- **Arquivamento e Portabilidade de Dados:**
  - Arquiva chamadas localmente no navegador (`localStorage`).
  - Exporta e importa dados em **JSON** e **CSV**.
  - Gera download em **PDF**.

## Como Usar

1. Extraia o arquivo `.zip`.
2. Abra o arquivo `index.html` em qualquer navegador moderno (Chrome, Edge, Firefox ou navegador mobile).
3. Clique nos campos desejados para colar os dados, revise o texto gerado e utilize os botões de copiar, WhatsApp, arquivar, exportar/importar ou baixar PDF.

## Histórico de Versões

- **Versão 1.0 - 21.11.26 - 03:43** — Versão inicial com colagem por clique, máscaras de Contrato e O.S., botão de limpeza de opção, formatação WhatsApp, arquivo local, importação/exportação JSON e CSV, exportação PDF e atalho de chamada para Tivit.

Criado por Fernando Sato - Versão 1.0 - 21.11.26 - 03:43
