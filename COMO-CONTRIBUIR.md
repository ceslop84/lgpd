# Como Contribuir

Adoraríamos receber sua ajuda! Este é um **projeto de código aberto e da comunidade**.

## 🤝 Formas de Contribuir

### 1. Reportar Problemas ou Sugestões

Encontrou um erro? Tem sugestão? Abra uma [Issue](https://github.com/seu-usuario/lgpd/issues)!

**Inclua:**
- Descrição clara do problema
- Contexto (qual página, que navegador)
- Screenshots se relevante

### 2. Melhorar Conteúdo

Você pode:
- ✏️ Corrigir erros de digitação
- 📚 Melhorar explicações confusas
- ➕ Adicionar novos tópicos
- 🌍 Traduzir para outro idioma

**Como:**
1. Fork o repositório
2. Crie uma branch: `git checkout -b melhoria/seu-topico`
3. Faça suas mudanças
4. Commit: `git commit -m "Melhorar [seção]: descrição"`
5. Push: `git push origin melhoria/seu-topico`
6. Abra um Pull Request (PR)

### 3. Melhorar Design

O site usa Jekyll com tema Minima. Sugestões:
- Novo layout
- Customizações CSS
- Melhor mobile responsiveness
- Acessibilidade

### 4. Traduzir

Quer deixar em outro idioma?
- Crie arquivos como `en/index.md` para cada idioma
- Atualize `_config.yml` para suportar multi-idioma

### 5. Divulgar

Compartilhar é contribuir!
- 📱 Compartilhe nas redes sociais
- 👥 Recomende para amigos
- 🎓 Use em sala de aula
- 📢 Mencione em posts/artigos

## 🔄 Processo de Pull Request

1. **Fork** o repositório
2. **Clone** seu fork: `git clone https://github.com/seu-usuario/lgpd.git`
3. **Crie branch**: `git checkout -b feature/sua-feature`
4. **Faça mudanças** e teste localmente
5. **Commit**: `git commit -m "Descrição clara"`
6. **Push**: `git push origin feature/sua-feature`
7. **Abra PR** no GitHub e descreva suas mudanças

## 📖 Diretrizes de Conteúdo

### Linguagem
- ✅ Simples, clara, acessível
- ✅ Evite jargão técnico (ou explique bem)
- ✅ Use exemplos práticos
- ✅ Português brasileiro

### Formatação
- Use Markdown
- Separe com headings (`##`, `###`)
- Use listas quando apropriado
- Adicione emojis para visual (com moderação)

### Precisão
- ✅ Cite fontes confiáveis
- ✅ Verifique antes de publicar
- ✅ Incluir datas quando relevante
- ✅ Corrigir erros promptamente

## 🧪 Testar Localmente

```bash
# Instalar dependências
bundle install

# Rodar servidor local
bundle exec jekyll serve

# Acessar http://localhost:4000
```

## 📝 Estrutura do Projeto

```
lgpd/
├── _config.yml           # Configuração Jekyll
├── Gemfile               # Dependências Ruby
├── index.md              # Página inicial
├── o-que-e-lgpd.md       # Explicação LGPD
├── direitos.md           # 10 direitos do cidadão
├── faq.md                # Perguntas frequentes
├── contato.md            # Formulário contato
├── README.md             # Este arquivo
├── GITHUB-PAGES-SETUP.md # Como deplorar
├── COMO-CONTRIBUIR.md    # Guia contribuição
└── assets/               # Imagens, CSS customizado
```

## 🎨 Modificar Estilo

Customize cores em `./_sass/custom.scss` (se usar Minima estendido):

```scss
$brand-color: #238636;
$text-color: #333;
```

## 🐛 Reportar Bug

1. Vá para [Issues](https://github.com/seu-usuario/lgpd/issues)
2. Clique em "New Issue"
3. Escolha template "Bug Report"
4. Preencha com detalhes

**Por favor inclua:**
- Sistema operacional
- Navegador e versão
- Passos para reproduzir
- O que esperava vs. o que aconteceu

## ✨ Sugerir Melhorias

1. Vá para [Issues](https://github.com/seu-usuario/lgpd/issues)
2. Clique em "New Issue"
3. Escolha template "Feature Request"
4. Descreva sua ideia

**A sugestão será melhor se:**
- For específica e clara
- Incluir exemplo de uso
- Explicar benefício

## 📚 Referências Úteis

- [Lei 13.709/2018](https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/L13709compilado.htm)
- [ANPD - Autoridade Nacional](https://www.gov.br/cidadania/pt-br/acesso-a-informacao/lgpd)
- [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/)
- [Jekyll Documentation](https://jekyllrb.com/docs/)

## 🙏 Agradecimentos

Obrigado por considerar contribuir!

Toda contribuição, grande ou pequena, melhora este projeto. Queremos tornar a proteção de dados acessível a TODOS.

---

**Código de Conduta:**
Todas as contribuições são bem-vindas. Por favor, seja respeitoso, tolerante e construtivo.

Se tiver dúvida: abra uma [Discussion](https://github.com/seu-usuario/lgpd/discussions) ou envie email via [formulário de contato](contato.html).
