# CLAUDE.md — ATELIERH2O

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** ATELIERH2O
**Nicho:** Casa e Decoração
**Keywords:** Seja muito bem vindo ao meu blog meu nome e Karina Machado
**Paleta de cores:** sunset | **Fonte:** lora

Seja muito bem vindo ao meu blog, meu nome é Karina Machado e esse é espaço que eu uso para falar sobre a minha paixão e experiência por arquitetura. Sinta-se em casa! Criei esse blog para dividir as minhas experiências, atuei por mais de 20 como arquiteta e quando comecei a me interessar por arquitetura, não tinha muito conteúdo disponível. Então decidi ajudar as pessoas que estão passando pelos mesmos problemas que eu. Minha maior motivação está em compartilhar tudo o que existe de mais relevante, bonito e interessante no universo da arquitetura, design, decoração e criatividade. Todos os leitores são muito bem vindos ao meu blog, dos níveis iniciantes ao avançado. Tenho diversos conteúdo para todos. Você vai encontrar análises técnicas sobre diversos assunto que envolvem arquitetura. Todas as análises são feitas com muita sabedoria e paixão antes de publicar.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-H |
| Hero | Hero-G |
| Features | Features-C |
| About Section | About-B |
| Posts | Posts-A |
| Footer | Footer-B |
| Página Sobre | Sobre-D |
| Página Contato | Contato-F |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
