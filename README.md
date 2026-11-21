# Automação de Ligação e WhatsApp — Sistema Tivit / Coop

Ferramenta web em arquivo único (`index.html`) voltada para técnicos de telecomunicações agilizar o repasse de informações durante ligações com o atendimento do sistema **Tivit / Coop**, formatar mensagens para **WhatsApp** e **arquivar os dados da chamada**.

---

## Funcionalidades

1. **Botão no topo para ligar para a Tivit**
   - Link direto `tel:+558007690800` no cabeçalho (`Ligar para Tivit (+558007690800)`).

2. **Cola automática ao clicar (`Nome do cliente`, `Endereço`, `WO`, `Contrato`)**
   - Ao clicar em qualquer um desses campos, o sistema lê a área de transferência (`navigator.clipboard.readText()`) e cola o conteúdo automaticamente.
   - Caso o navegador bloqueie a leitura direta da área de transferência, o campo recebe foco para colagem manual (`Ctrl+V` ou toque em **Colar**).

3. **Formatação e destaque visual de WO e Contrato**
   - **WO:** formatado como `xxx.xxx.xxx` com fonte ampliada.
   - **Contrato:** formatado como `xxx.xxx.xxx` com fonte ampliada.

4. **Formatação e envio para WhatsApp**
   - **Formatar para WhatsApp:** monta a mensagem com os dados fixos do atendimento e variáveis na sequência configurada.
   - **Formatar e abrir WhatsApp:** gera a mensagem e abre o link `https://wa.me/?text=...`.
   - **Copiar mensagem:** copia o texto formatado para a área de transferência.

5. **Arquivamento de dados da chamada**
   - **Arquivar dados da chamada:** salva o registro com data e hora no armazenamento local do navegador (`localStorage`), permitindo **Carregar** novamente nos campos, **Copiar Wpp**, **Excluir**, **Baixar arquivo (.txt)** ou **Limpar arquivo**.

---

## Como usar

1. Extraia o arquivo `.zip`.
2. Abra o arquivo `index.html` diretamente no navegador (Chrome, Edge, Safari etc.).
3. Use o botão do topo para ligar para a Tivit (`+558007690800`), se necessário.
4. Copie cada informação necessária e clique no campo correspondente para colar.
5. Use o roteiro na ligação, formate para WhatsApp e clique em **Arquivar dados da chamada** ao finalizar.

---

## Histórico de versões

- **Versão 1.5 - 21.11.26 - 02:01:** Formatação do campo WO no padrão `xxx.xxx.xxx`, aumento do tamanho da fonte dos números de WO e de Contrato (campos, roteiro e chamadas arquivadas) e atualização do `README.md`.
- **Versão 1.4 - 21.11.26 - 01:55:** Adição do botão no topo para ligar para Tivit (`+558007690800`), máscaras de exibição para Contrato (`xxx.xxx.xxx`) e WO (`xxx. xxx.xxx.xxxx`), remoção do bloco `4. Dados fixos` na interface e atualização do `README.md`.
- **Versão 1.3 - 21.11.26 - 01:34:** Inclusão do botão **Arquivar dados da chamada**, histórico com carregar/copiar/excluir/exportar `.txt` e inclusão do `README.md` no pacote `.zip`.
- **Versão 1.2 - 21.11.26 - 01:32:** Cola automática da área de transferência ao clicar nos campos variáveis e inclusão dos dados fixos do sistema Tivit / Coop.
- **Versão 1.1 - 21.11.26 - 01:17:** Padronização do arquivo principal como `index.html` no `.zip`.
- **Versão 1.0 - 21.11.26 - 00:14:** Versão inicial com campos de atendimento e formatação para WhatsApp.

---

Criado por Fernando Sato - Versão 1.5 - 21.11.26 - 02:01
