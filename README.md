# Automação de Ligação e WhatsApp — Sistema Tivit / Coop

Ferramenta web em arquivo único (`index.html`) voltada para técnicos de telecomunicações agilizar o repasse de informações durante ligações com o atendimento do sistema **Tivit / Coop**, formatar mensagens para **WhatsApp** e **arquivar os dados da chamada**.

---

## Funcionalidades

1. **Botão no topo para ligar para a Tivit**
   - Link direto `tel:+558007690800` no cabeçalho (`Ligar para Tivit (+558007690800)`).

2. **Cola automática ao tocar/clicar (`Nome do cliente`, `Endereço`, `O.S`, `Contrato`)**
   - Ao tocar ou clicar em qualquer um desses campos, o sistema tenta ler a área de transferência (`navigator.clipboard.readText()`) e aplicar a formatação automaticamente no campo, no roteiro e na prévia.
   - Caso o navegador exija permissão ou bloqueie a leitura direta em visualização/arquivo local, o campo recebe foco e intercepta o evento `paste` (`Ctrl+V` ou toque em **Colar**) para formatar e atualizar o roteiro automaticamente.
   - Abaixo de cada um dos 4 campos (`Nome do cliente`, `Endereço`, `O.S`, `Contrato`), há um botão pequeno **Limpar campo** para apagar rapidamente caso alguma informação incorreta seja colada.

3. **Formatação e destaque visual de Nome, Endereço, O.S e Contrato**
   - **O.S:** formatado como `xxx.xxx.xxxx` com fonte ampliada.
   - **Contrato:** formatado como `xxx.xxx.xxx` com fonte ampliada.
   - **Nome do cliente** e **Endereço:** exibidos com fonte ampliada no campo, no roteiro e nas chamadas arquivadas.

4. **Formatação e envio para WhatsApp**
   - **Formatar para WhatsApp:** monta a mensagem com os dados fixos do atendimento e variáveis na sequência configurada.
   - **Formatar e abrir WhatsApp:** gera a mensagem e abre o link `https://wa.me/?text=...`.
   - **Copiar mensagem:** copia o texto formatado para a área de transferência.

5. **Arquivamento, Importação, Exportação (JSON / CSV) e Download em PDF**
   - **Arquivar dados da chamada:** salva o registro com data e hora no armazenamento local do navegador (`localStorage`), permitindo **Carregar** novamente nos campos, **Copiar Wpp** ou **Excluir**.
   - **Exportar JSON / Importar JSON:** salva e restaura o histórico em arquivo `.json` (`chamadas-arquivadas-tivit-coop.json`).
   - **Exportar CSV / Importar CSV:** salva em planilha compatível com Excel (`chamadas-arquivadas-tivit-coop.csv`) e importa registros de arquivos `.csv`.
   - **Baixar PDF:** gera e baixa diretamente um relatório em PDF (`chamadas-arquivadas-tivit-coop.pdf`) com os registros arquivados.
   - **Baixar (.txt) / Limpar arquivo:** exporta o histórico em texto simples ou limpa os registros salvos.

---

## Como usar

1. Extraia o arquivo `.zip`.
2. Abra o arquivo `index.html` diretamente no navegador (Chrome, Edge, Safari etc.).
3. Use o botão do topo para ligar para a Tivit (`+558007690800`), se necessário.
4. Copie cada informação necessária e toque/clique no campo correspondente para colar (ou use `Ctrl+V` / **Colar** e **Limpar campo** se precisar corrigir).
5. Use o roteiro na ligação, formate para WhatsApp, arquive a chamada e utilize os botões de **JSON**, **CSV**, **PDF** ou **.txt** conforme necessário.

---

## Histórico de versões

- **Versão 1.11 - 21.11.26 - 02:48:** Reforço na leitura da área de transferência no toque/clique (`pointerdown`), tratamento do evento `paste` para formatação imediata e atualização do `README.md`.
- **Versão 1.10 - 21.11.26 - 02:39:** Adição de **Exportar JSON**, **Importar JSON**, **Exportar CSV**, **Importar CSV** e **Baixar PDF** na seção de chamadas arquivadas, além da atualização do `README.md`.
- **Versão 1.9 - 21.11.26 - 02:26:** Formatação do campo `O.S` no padrão `xxx.xxx.xxxx`, aumento do tamanho da fonte de `Nome do cliente`, `Endereço`, `O.S` e `Contrato`, e atualização do `README.md`.
- **Versão 1.8 - 21.11.26 - 02:18:** Remoção do prefixo `O.S` do valor formatado e alteração do rótulo `WO` para `O.S` (formato `xxx.xxx.xxx` com fonte ampliada), e atualização do `README.md`.
- **Versão 1.7 - 21.11.26 - 02:14:** Formatação do campo WO no padrão `O.S xxx.xxx.xxxx` (mantendo fonte ampliada), ajuste no roteiro, mensagem do WhatsApp e chamadas arquivadas, e atualização do `README.md`.
- **Versão 1.6 - 21.11.26 - 02:06:** Inclusão de botão pequeno **Limpar campo** abaixo de cada um dos 4 campos (`Nome do cliente`, `Endereço`, `WO` e `Contrato`) e atualização do `README.md`.
- **Versão 1.5 - 21.11.26 - 02:01:** Formatação do campo WO no padrão `xxx.xxx.xxx`, aumento do tamanho da fonte dos números de WO e de Contrato (campos, roteiro e chamadas arquivadas) e atualização do `README.md`.
- **Versão 1.4 - 21.11.26 - 01:55:** Adição do botão no topo para ligar para Tivit (`+558007690800`), máscaras de exibição para Contrato (`xxx.xxx.xxx`) e WO (`xxx. xxx.xxx.xxxx`), remoção do bloco `4. Dados fixos` na interface e atualização do `README.md`.
- **Versão 1.3 - 21.11.26 - 01:34:** Inclusão do botão **Arquivar dados da chamada**, histórico com carregar/copiar/excluir/exportar `.txt` e inclusão do `README.md` no pacote `.zip`.
- **Versão 1.2 - 21.11.26 - 01:32:** Cola automática da área de transferência ao clicar nos campos variáveis e inclusão dos dados fixos do sistema Tivit / Coop.
- **Versão 1.1 - 21.11.26 - 01:17:** Padronização do arquivo principal como `index.html` no `.zip`.
- **Versão 1.0 - 21.11.26 - 00:14:** Versão inicial com campos de atendimento e formatação para WhatsApp.

---

Criado por Fernando Sato - Versão 1.11 - 21.11.26 - 02:48
