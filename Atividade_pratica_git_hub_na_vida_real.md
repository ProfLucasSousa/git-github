# Atividade Prática – GitHub na Vida Real

## Contexto
Nesta atividade você vai usar **GitHub de verdade**, seguindo um fluxo parecido com o de times profissionais. Nada de simulação local: tudo acontece no repositório público do professor.

Repositório base:
👉 https://github.com/ProfLucasSousa/git-github.git

---

## Objetivo da atividade
Ao final, você deverá provar que sabe:

- Interagir com um repositório público
- Trabalhar com **fork**, **clone** e **branch**
- Fazer **commits semânticos**
- Enviar código para o GitHub
- Abrir **Pull Request** corretamente

Se errar, faz parte. Se não versionar, aí sim é erro.

---

## Etapa 1 – Star no repositório ⭐

1. Acesse o repositório
2. Clique em **Star**

Simples, mas obrigatório. GitHub também é vitrine.

---

## Etapa 2 – Fork do repositório 🍴

1. Clique em **Fork**
2. Crie uma cópia do repositório na sua conta

A partir daqui, o projeto é **seu**, mas a origem continua sendo o repositório do professor.

---

## Etapa 3 – Clone remoto

Clone o repositório forkado (o da sua conta):

```bash
git clone https://github.com/SEU_USUARIO/git-github.git
cd git-github
```

Verifique o remote:

```bash
git remote -v
```

Você deve ver o `origin` apontando para o seu fork.

---

## Etapa 4 – Criar uma branch

Nada de trabalhar na `main`.

Crie uma branch com seu nome:

```bash
git checkout -b feat/seu-nome
```

Exemplo:

```bash
git checkout -b feat/lucas-sousa
```

---

## Etapa 5 – Modificar ou adicionar conteúdo

Escolha **uma** das opções abaixo:

### Opção A – Adicionar seu nome

- Crie ou edite o arquivo `ALUNOS.md`
- Adicione:
  - Seu nome
  - Curso
  - Uma frase curta (sem texto motivacional, por favor)

### Opção B – Melhorar o README

- Corrija texto
- Organize seções
- Acrescente uma explicação clara sobre o objetivo do repositório

---

## Etapa 6 – Commit semântico

Adicione os arquivos:

```bash
git add .
```

Faça **um commit semântico**:

```bash
git commit -m "feat(alunos): adiciona informações do aluno"
```

Ou:

```bash
git commit -m "docs(readme): melhora explicação do projeto"
```

Commits genéricos tipo `update` não contam.

---

## Etapa 7 – Push para o GitHub

Envie sua branch:

```bash
git push origin feat/seu-nome
```

Se isso falhar, você pulou alguma etapa.

---

## Etapa 8 – Abrir Pull Request

1. Vá até seu fork no GitHub
2. Clique em **Compare & Pull Request**
3. Preencha:
   - Título claro
   - Descrição curta do que foi feito

O PR deve apontar:
- **Base**: repositório do professor
- **Compare**: sua branch

---

## Etapa 9 – Criar uma Issue (extra)

Crie **uma issue** no repositório original com:

- Título objetivo
- Sugestão de melhoria real

Exemplo:
> Sugestão: adicionar seção de contribuição no README

---

## Etapa 10 – Atualizar o fork (extra)

Depois do PR, sincronize seu fork com o original.

(Entender isso agora evita dor de cabeça depois.)

---

## Critérios de avaliação

✔ Deu star no repositório
✔ Fez fork corretamente
✔ Usou branch
✔ Commit semântico
✔ Push funcionando
✔ Pull Request aberto corretamente

Extras contam ponto.

---

## Observações finais

- PR sem descrição = retrabalho
- Commit mal escrito = histórico inútil
- Push direto na `main` = erro clássico

Essa atividade não é sobre decorar comando.
É sobre **trabalhar como dev de verdade**.

