# Automação de Ligação e WhatsApp — Sistema Tivit / Coop

Aplicação web em arquivo único (`index.html`) baseada no layout escuro (`Versão 1.2`) com as funcionalidades de atendimento e registro de chamadas.

## Comparação com o Arquivo Enviado (`Versão 1.2`)

- **Base visual e estrutural mantida:** Mesmo esquema de cores escuras (`#0f172a`, `#1e293b`, `#0b1220`, `#38bdf8`, `#22c55e`), cards e fluxo de colagem ao clicar.
- **No arquivo enviado (`Versão 1.2`):**
  - Não havia botão de ligação para `+558007690800` no topo.
  - Não havia campo/botão para limpar **Opção** separadamente.
  - **WO** e **Contrato** não aplicavam máscaras (`xxx.xxx.xxx.xxxx` e `xxx.xxx.xxx`).
  - Não havia arquivamento de chamadas, importação/exportação **JSON** e **CSV**, nem exportação **PDF**.
  - O rodapé marcava `Versão 1.2 - 21.11.26 - 01:32`.
- **Adicionado nesta versão (`Versão 1.3 - 21.11.26 - 03:57`):**
  - Botão de ligação no topo para `+558007690800` (`tel:+558007690800`).
  - Campo **Opção / Observação** com botão **Limpar campo opção** logo abaixo.
  - Máscaras automáticas em **WO / O.S.** (`xxx.xxx.xxx.xxxx`) e **Contrato** (`xxx.xxx.xxx`).
  - Arquivamento local de chamadas, importação/exportação **JSON** e **CSV**, e geração de **PDF**.
  - Rodapé e documentação atualizados para `Versão 1.3 - 21.11.26 - 03:57`.

## Por que a leitura automática da área de transferência pode falhar no navegador

Mesmo com o clique no campo, navegadores modernos bloqueiam `navigator.clipboard.readText()` quando o arquivo HTML é aberto diretamente por `file://` (duplo clique no arquivo) ou sem permissão/HTTPS. Quando isso ocorre, o campo recebe foco e exibe o aviso para usar `Ctrl+V` / **Colar**, e o evento `paste` formata o texto automaticamente.

Criado por Fernando Sato - Versão 1.3 - 21.11.26 - 03:57
