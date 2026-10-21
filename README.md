# Controle de Documentos - MBernardes Advocacia

## Sobre o projeto

Aplicação web acadêmica e responsiva para auxiliar advogados, estagiários e colaboradores administrativos no acompanhamento de documentos solicitados e recebidos em atendimentos jurídicos.

O projeto registra apenas informações de acompanhamento, como cliente/atendimento, documento solicitado, data e situação. **Não armazena os arquivos dos documentos.**

## Funcionalidades

- Cadastro de cliente/atendimento e documento solicitado, com data automática.
- Pesquisa de registros pelo nome do cliente, atualizada durante a digitação.
- Alteração do status de cada registro entre **Pendente** e **Recebido**.
- Exclusão de registros.
- Persistência dos registros no navegador por meio do `localStorage`.
- Layout adaptável a diferentes tamanhos de tela, com tabela responsiva.

## Tecnologias utilizadas

- **HTML5:** estrutura da página, formulário e tabela.
- **Bootstrap 5.3.0:** framework de interface, layout e componentes responsivos.
- **Bootstrap Icons 1.10.5:** ícones da interface.
- **JavaScript:** cadastro, pesquisa, atualização do status, exclusão e armazenamento local.
- **Web Storage API (`localStorage`):** persistência dos dados no navegador.

O estilo é fornecido predominantemente pelas classes do Bootstrap. O JavaScript está incorporado ao arquivo `index.html`, sem necessidade de arquivos separados `style.css` ou `app.js` nesta versão.

## Arquivos

```text
index.html  - interface, estrutura e funcionalidades da aplicação
README.md   - documentação do projeto
```

## Como executar

1. Baixe os arquivos do repositório.
2. Abra `index.html` em um navegador moderno.
3. Cadastre um documento para acompanhar seu status.

Não é necessário instalar um servidor ou configurar um banco de dados. **É preciso acesso à internet para carregar os estilos e ícones do Bootstrap a partir das CDNs.**

## Decisões de desenvolvimento

O projeto utiliza Bootstrap para simplificar a construção de uma interface responsiva, JavaScript no navegador para executar as operações interativas e `localStorage` para persistência local sem infraestrutura de servidor. A escolha atende ao escopo demonstrativo e reduz a complexidade de instalação.

## Limites e cuidados

- Os dados permanecem apenas no navegador/dispositivo utilizado; não existe sincronização entre usuários.
- O sistema não possui autenticação, controle de acesso ou banco de dados centralizado.
- A exclusão de registros não solicita confirmação.
- O projeto é um **protótipo acadêmico**: utilize apenas dados fictícios, nunca informações reais ou sigilosas de clientes.

## Público-alvo

Advogados, estagiários e colaboradores administrativos de escritórios de advocacia que acompanham solicitações documentais.
