# Portfólio — Débora Rodrigues

Site estático (HTML puro), pronto para publicar no Vercel via GitHub.

## Estrutura

```
portfolio/
├── index.html              → apresentação Cash.Tools (deborarodrigues.vercel.app)
├── cash-tools/
│   └── cash-tools-5min.html → versão 5 min, página única (…/cash-tools/cash-tools-5min.html)
├── vercel.json             → redireciona o endereço antigo /cash-tools/ para a página inicial
└── README.md               → este guia
```

Cada novo case vira uma pasta com um `index.html` dentro, por exemplo `outro-case/index.html` → `…/outro-case`.

---

## Passo a passo para publicar

### 1. Criar o repositório no GitHub

1. Entre em [github.com](https://github.com) (crie a conta, se ainda não tiver).
2. Clique em **+** (canto superior direito) → **New repository**.
3. Em *Repository name*, escreva `portfolio`.
4. Marque **Public**. Não marque nenhuma outra opção.
5. Clique em **Create repository**.

### 2. Subir os arquivos

1. Na página do repositório recém-criado, clique no link **uploading an existing file**.
2. Descompacte o `.zip` no seu computador e **arraste o conteúdo da pasta** `portfolio` (o `index.html`, a pasta `cash-tools` e o `README.md`) para a área de upload.
   - Importante: o `index.html` precisa ficar na raiz do repositório, e não dentro de uma subpasta `portfolio/`.
   - Arraste pelo Finder/Explorador de Arquivos para a pasta `cash-tools` ir junto.
3. Clique em **Commit changes**.

### 3. Conectar ao Vercel

1. Entre em [vercel.com](https://vercel.com) → **Sign Up** → **Continue with GitHub**.
   Se pedir, escolha o plano **Hobby** (gratuito, uso pessoal).
2. Autorize o Vercel a acessar seu GitHub (pode liberar só o repositório `portfolio`).
3. No painel, clique em **Add New… → Project**.
4. Ao lado do repositório `portfolio`, clique em **Import**.
5. Na tela de configuração:
   - **Project Name**: escolha o nome que vai aparecer no link, por exemplo `deborarodrigues` → `deborarodrigues.vercel.app`.
   - **Framework Preset**: deixe **Other**.
   - Não precisa mudar mais nada.
6. Clique em **Deploy**. Em cerca de um minuto o site estará no ar.

### 4. Ajustar o endereço (opcional)

- **Trocar o nome depois:** Project → **Settings → Domains** → edite o domínio `.vercel.app`, se o nome estiver livre.
- **Domínio próprio** (ex.: `deborarodrigues.com.br`): compre o domínio no [registro.br](https://registro.br), adicione-o em **Settings → Domains** e siga as instruções de DNS que o Vercel mostrar.

---

## Como atualizar o site

Toda alteração enviada ao GitHub publica o site de novo, sozinha.

1. No GitHub, abra o arquivo (ex.: `index.html`) → ícone de lápis para editar, ou **Add file → Upload files** para substituir.
2. **Commit changes**.
3. Em cerca de um minuto, o Vercel publica a nova versão.

---

## Antes de divulgar o link

Ainda há placeholders na página inicial:

- [ ] Cards 02 e 03 da seção **Trabalho selecionado** (trocar por cases reais ou remover)
- [ ] Texto da seção **Sobre**
- [ ] Links do **LinkedIn** e do **Currículo** (hoje apontam para `#`)
- [ ] Frase do rodapé ("Rascunho gerado com Claude…")
- [ ] Revisar se o e-mail de contato deve ser o da Rebase ou um pessoal
