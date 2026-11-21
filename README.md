# Automação de Ligação e WhatsApp — Sistema Tivit / Coop

Ferramenta web em arquivo único (`index.html`) voltada para técnicos de telecomunicações agilizar o repasse de informações durante ligações com o atendimento do sistema **Tivit / Coop**, formatar mensagens para **WhatsApp** e **arquivar os dados da chamada**.

---

## Funcionalidades

1. **Cola automática ao clicar (`Nome do cliente`, `Endereço`, `WO`, `Contrato`)**
   - Ao clicar em qualquer um desses campos, o sistema lê a área de transferência (`navigator.clipboard.readText()`) e cola o conteúdo automaticamente.
   - Caso o navegador bloqueie a leitura direta da área de transferência, o campo recebe foco para colagem manual (`Ctrl+V` ou toque em **Colar**).

2. **Dados fixos mantidos na ordem do atendimento**
   - **Opção do serviço:** `239`
   - **Cidade:** `003`
   - **Código da empresa:** `68804663#`
   - **Nome do Funcionário:** `Fernando Sato`
   - **Código Funcionário:** `Z688632`
   - **Nome da Conveniada:** `CSR Engenharia Ltda`
   - **PDA:** `91520-6585`
   - **Código da Baixa:** `409`
   - **Tipo de wo:** `Instalação/	Mudança de Pacote`
   - **Hora de Início:** `12:00`

3. **Formatação e envio para WhatsApp**
   - **Formatar para WhatsApp:** monta a mensagem com os dados fixos e variáveis na sequência configurada.
   - **Formatar e abrir WhatsApp:** gera a mensagem e abre o link `https://wa.me/?text=...`.
   - **Copiar mensagem:** copia o texto formatado para a área de transferência.

4. **Arquivamento de dados da chamada**
   - **Arquivar dados da chamada:** salva o registro com data e hora no armazenamento local do navegador (`localStorage`), permitindo **Carregar** novamente nos campos, **Copiar Wpp**, **Excluir**, **Baixar arquivo (.txt)** ou **Limpar arquivo**.

---

## Como usar

1. Extraia o arquivo `.zip`.
2. Abra o arquivo `index.html` diretamente no navegador (Chrome, Edge, Safari etc.).
3. Copie cada informação necessária e clique no campo correspondente para colar.
4. Use o roteiro na ligação, formate para WhatsApp e clique em **Arquivar dados da chamada** ao finalizar.

---

## Histórico de versões

- **Versão 1.3 - 21.11.26 - 01:34:** Inclusão do botão **Arquivar dados da chamada**, histórico com carregar/copiar/excluir/exportar `.txt` e inclusão do `README.md` no pacote `.zip`.
- **Versão 1.2 - 21.11.26 - 01:32:** Cola automática da área de transferência ao clicar nos campos variáveis e inclusão dos dados fixos do sistema Tivit / Coop.
- **Versão 1.1 - 21.11.26 - 01:17:** Padronização do arquivo principal como `index.html` no `.zip`.
- **Versão 1.0 - 21.11.26 - 00:14:** Versão inicial com campos de atendimento e formatação para WhatsApp.

---

Criado por Fernando Sato - Versão 1.3 - 21.11.26 - 01:34
