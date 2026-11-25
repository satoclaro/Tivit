# Automação de Ligação e WhatsApp — Sistema Tivit / Coop

Aplicação web mobile-first (Dark Theme) desenvolvida para agilizar o atendimento e a baixa de Ordens de Serviço (O.S) junto à central **Tivit / Coop**.

## Funcionalidades

- **Discagem Rápida no Topo:** Botão de chamada direta (`tel:+558007690800`) para acionar a central Tivit com um toque.
- **Cola Automática (One-Tap Clipboard):** Ao tocar nos campos **Nome do cliente**, **Endereço**, **O.S** ou **Contrato**, o conteúdo da área de transferência é colado automaticamente.
- **Formatação Padronizada e Leitura Ampliada:**
  - **Contrato** formatado automaticamente no padrão `xxx.xxx.xxx`.
  - **O.S (WO)** formatada automaticamente no padrão `xxx.xxx.xxxx`.
  - Exibição em cartões de destaque com **fonte ampliada** após a formatação para facilitar a leitura durante a ligação.
- **Integração com WhatsApp:** Monta a mensagem na ordem exata exigida pelo fluxo operacional com envio direto via `wa.me` ou cópia rápida.
- **Roteiro em Tempo Real:** Atualiza a lista de leitura passo a passo para a atendente conforme os dados são inseridos.
- **Arquivamento Local e Exportação/Importação:**
  - Salva chamadas no navegador (`localStorage`).
  - Exportação e importação completa em **JSON** e **CSV**.
  - Geração e download de relatório tabular em **PDF**.

## Como Usar

1. Abra o arquivo `index.html` em um navegador moderno (preferencialmente hospedado via HTTPS no GitHub Pages para liberar leitura direta da área de transferência no Android/Chrome).
2. Toque no botão **Ligar Tivit: +55 800 769 0800** no cabeçalho para iniciar a chamada.
3. Copie os dados da O.S no sistema de campo e toque em cada campo correspondente para colar.
4. Clique em **Formatar** para visualizar o **Contrato** (`xxx.xxx.xxx`) e a **O.S** (`xxx.xxx.xxxx`) em fonte maior e gerar o texto do WhatsApp.
5. Utilize **Arquivar Chamada** para registrar o atendimento no histórico e exportar em **JSON**, **CSV** ou **PDF** quando necessário.

---
Criado por: Fernando Sato - Versão 1.1 - 24/11/2026 20:37
