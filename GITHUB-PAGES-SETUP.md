# Guia de Setup - GitHub Pages + Execução Local

Este guia reúne tudo o que você precisa para:
- Publicar o site no **GitHub Pages**
- Testar e desenvolver localmente com **Jekyll**

## 📋 Pré-requisitos

- [GitHub](https://github.com) account
- [Git](https://git-scm.com/) instalado
- [Ruby](https://www.ruby-lang.org/) versão 2.7+

## 🧩 Instalar Ruby (Linux / macOS)

### Linux (Ubuntu/Debian)

```bash
sudo apt update
sudo apt install -y ruby ruby-dev build-essential

# Verificar instalação
ruby --version
```

### macOS

```bash
brew install ruby
ruby --version
```

> Se você já tem Ruby instalado, basta confirmar a versão.


## 🧶 Instalar Bundler (gerenciador de gemas)

```bash
gem install bundler
bundle --version
```


## 📦 Instalar dependências do projeto

No diretório do projeto (`/home/ceslop84/git/lgpd`):

```bash
cd /home/ceslop84/git/lgpd
bundle install
```

Isso instalará o Jekyll e os plugins definidos em `Gemfile`.


## 🚀 Passo 1: Push para GitHub

Se ainda não fez, faça push do repositório local para GitHub:

```bash
cd /home/ceslop84/git/lgpd
git add .
git commit -m "Adicionar website LGPD com Jekyll"
git push origin main
```


## 🔧 Passo 2: Configurar GitHub Pages

1. Vá para: **Settings** → **Pages**
2. Em "Source", selecione:
   - **Branch**: `main` (ou `master`)
   - **Folder**: `/ (root)`
3. Clique em **Save**

GitHub Pages começará o build automático!


## ⚙️ Passo 3: Atualizar `_config.yml` (IMPORTANTE!)

Abra `_config.yml` e descomente as linhas de URL:

```yaml
# URL for GitHub Pages
url: "https://seu-usuario-github.github.io"
baseurl: "/lgpd"  # Se o repo for 'lgpd', senão deixe vazio
```

**Exemplos:**
- Se repo é `seu-usuario.github.io`: `baseurl: ""`
- Se repo é `seu-usuario/lgpd`: `baseurl: "/lgpd"`

Depois:
```bash
git add _config.yml
git commit -m "Atualizar configuração de URL"
git push origin main
```


## 📱 Visualizar Site

Após alguns minutos, acesse:
- Se repo é `seu-usuario.github.io`: `https://seu-usuario.github.io`
- Se repo é `seu-usuario/lgpd`: `https://seu-usuario.github.io/lgpd`


## 🧪 Testar Localmente (Recomendado)

Para visualizar antes de fazer push:

```bash
cd /home/ceslop84/git/lgpd

# Instalar dependências (se não fez ainda)
bundle install

# Rodar servidor local
bundle exec jekyll serve

# Acesse: http://localhost:4000
```

O site atualiza automaticamente quando você salva alterações nos arquivos.


## 🧪 Testar em Pasta `pages/`

O conteúdo do site está em `pages/` e os URLs não mudaram porque cada página usa `permalink`.

Se quiser adicionar nova página:

1. Crie o arquivo em `pages/` (por exemplo `pages/nova-pagina.md`)
2. Adicione front matter:
   ```yaml
   ---
   layout: default
   title: Nova Página
   permalink: /nova-pagina.html
   ---
   ```
3. Confirme que está listado em `_config.yml` (header_pages)


## 🎨 Customizações

### Trocar Tema

Edite `_config.yml`:
```yaml
theme: minima  # Trocar para outro tema
```

**Temas populares:**
- `minima` (padrão)
- `jekyll-theme-cayman`
- `jekyll-theme-slate`
- `jekyll-theme-modernist`

Depois reinicie o build.

### Adicionar Favicon

Coloque um `favicon.ico` na raiz do projeto:

```
lgpd/
├── favicon.ico
├── pages/
└── ...
```

### Adicionar Logo

Crie pasta `assets/images/` e coloque um logo chamado `logo.png`.

Em `_config.yml`:
```yaml
logo: /assets/images/logo.png
```


## 📧 Configurar Formulário de Contato

O formulário usa [Formspree](https://formspree.io/) (gratuito):

1. **Acesse:** [https://formspree.io/register](https://formspree.io/register)
2. **Crie uma conta** com seu email
3. **Crie um novo formulário:**
   - Dê um nome (ex: "LGPD - Contato")
   - Adicione seu email para receber as mensagens
4. **Copie o código do formulário** (parece algo como `xyzabc123`)
5. **Substitua** `seu-codigo-aqui` no arquivo `pages/contato.md` pelo código real
6. **Faça commit e push** para o GitHub

**Exemplo:**
```html
<form action="https://formspree.io/f/xyzabc123" method="POST">
```

**Resultado esperado:** Após configurar, você receberá emails quando alguém enviar o formulário.


## 🔍 Verificar Erros

Se o site não aparecer, verifique:

1. **Settings → Pages**: Branch e folder estão corretos?
2. **Actions**: Há erro no build? (veja Actions tab no GitHub)
3. **_config.yml**: URL e baseurl estão corretos?
4. **Sintaxe**: Algum erro em Markdown?


## 🎯 Próximos Passos

- ✅ Configure GitHub Pages
- ✅ Teste o site online
- ✅ Configure formulário de contato
- ✅ Customize logo e cores
- ✅ Compartilhe o link!


## 📚 Recursos

- [Documentação Jekyll](https://jekyllrb.com/)
- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [Minima Theme](https://github.com/jekyll/minima)

---

**Dúvida?** Consulte o arquivo README.md ou envie uma mensagem na página de contato!
