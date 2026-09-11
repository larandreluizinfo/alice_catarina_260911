# AGENTS — Regras do repositório

## Git: commit + push obrigatório

- Toda alteração em arquivo deve ser commitada e pushada para o GitHub.
- Nunca deixe alterações apenas locais / não commitadas ao final de uma tarefa.
- Fluxo obrigatório após qualquer edição/criação/remoção de arquivos:
  1. `git status` para conferir o que mudou
  2. `git add -A`
  3. `git commit -m "<mensagem clara>"`
  4. `git push origin main` (ou `git push` se o upstream já estiver configurado)
- Se o `push` falhar (sem remote, sem auth, branch nova), resolver na hora:
  - sem remote → avisar e configurar `origin`
  - sem auth → pedir `gh auth login`
  - branch sem upstream → `git push -u origin main`
- Não pule o push alegando falta de mudança relevante: se houve edit em arquivo rastreado, tem que commitar + pushar.
- Mensagens de commit em português, curtas e descritivas.
