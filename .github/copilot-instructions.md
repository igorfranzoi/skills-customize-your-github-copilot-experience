# Descrição do Projeto

Este projeto é um site educacional para compartilhar tarefas de casa e exercícios de programação com estudantes. Os estudantes podem navegar, visualizar e baixar tarefas diretamente do portal.

## Estrutura do Projeto

- [`assignments/`](../assignments/) Cada tarefa de casa é armazenada em sua própria subpasta com uma estrutura consistente.
- [`templates/`](../templates/) Templates reutilizáveis para novo conteúdo
- [`assets/`](../assets/) Contém os recursos do site incluindo CSS, JavaScript, imagens e arquivos de configuração
- [`index.html`](../index.html) A página principal do site que serve como um portal estático para navegar e visualizar tarefas. O conteúdo é configurável através do arquivo [`config.json`](../config.json) para gerar dinamicamente listas e detalhes de tarefas.

## Diretrizes do Projeto

- Manter estilo consistente em todas as páginas
- Manter nomes de arquivos e pastas descritivos e organizados

## Padrões Educacionais

Ao gerar conteúdo para este projeto:

- **Focado em aprendizado**: Todo conteúdo deve ser projetado com objetivos de aprendizado claros e níveis de dificuldade apropriados
- **Amigável para estudantes**: Use linguagem clara e encorajadora que motiva os estudantes

## Commits Convencionais

Usamos Conventional Commits para manter o histórico de commits claro e automatizar releases.  
Formato básico:
<type>[optional scope]: <descrição curta>

Opções comuns de type:
- feat: nova funcionalidade
- fix: correção de bug
- docs: documentação
- style: formatação/código sem alterar lógica
- refactor: refatoração de código
- perf: melhoria de performance
- test: adicionar/ajustar testes
- chore: tarefas de manutenção (deps, scripts)
- build: alterações no processo de build
- ci: alterações de CI/CD
- revert: reverter um commit

Breaking change:
- Indique com "!" após o type/scope: feat!: mudança incompatível
- Inclua um rodapé com "BREAKING CHANGE: descrição"

Exemplos:
- feat(auth): adicionar login via OAuth
- fix(api): tratar resposta nula no endpoint /users
- docs(readme): atualizar instruções de setup
- style: aplicar prettier no projeto
- refactor(session): simplificar lógica de sessão
- perf(db): otimizar consulta de relatórios
- test: adicionar testes unitários para utils
- chore(deps): atualizar dependências de desenvolvimento
- build: ajustar configuração do webpack
- ci(github): adicionar workflow de lint

Exemplo com corpo e breaking change:
feat(config)!: mudar formato do arquivo de configuração

Altera o parser para aceitar o novo formato de configuração com objetos aninhados.

BREAKING CHANGE: arquivos de configuração antigos não são mais compatíveis; atualizar para o novo formato.