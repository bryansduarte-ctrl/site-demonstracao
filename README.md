# Site Demonstração — AutoEscola ViaLivre

Landing page modelo usada como **demonstração** para prospecção de autoescolas.
Fictícia (AutoEscola ViaLivre, Santo André-SP) — serve de vitrine do trabalho do Cérebro.

- **Repositório:** https://github.com/bryansduarte-ctrl/site-demonstracao
- **Deploy:** Vercel (auto-deploy a cada push na branch `main`)
- **Arquivo único:** `index.html` (HTML + CSS + JS inline, sem dependências)

---

## Identidade visual

- **Azul profundo** `#0F2347` / `#1A3A6C` — confiança, seriedade
- **Amarelo** `#F5C518` — destaque, energia (CNH / trânsito)
- **Verde WhatsApp** `#25D366` — todos os CTAs de contato
- Fontes: Barlow Condensed (títulos) + Inter (texto)

---

## Estrutura da página

1. Nav fixo + menu hambúrguer (mobile)
2. Hero com card de orçamento (form → WhatsApp)
3. Categorias de CNH (grid 3×2 no desktop)
4. Como funciona (3 passos)
5. Por que escolher (diferenciais)
6. Depoimentos
7. **FAQ** (acordeão `<details>`, 6 perguntas)
8. CTA banner
9. Localização (mapa + contato)
10. Footer + redes sociais
11. Botão flutuante de WhatsApp

---

## Recursos técnicos

- Responsivo (breakpoints 900px e 600px)
- Animações de scroll suaves (IntersectionObserver + stagger)
- `prefers-reduced-motion` respeitado
- **SEO:** meta description, Open Graph (preview no WhatsApp), Twitter Card
- **Dados estruturados (JSON-LD):** `DrivingSchool` + `FAQPage` — ajuda no Google, Maps e IAs (GEO)

---

## ⚠️ Antes de usar com um cliente real

Trocar os placeholders:

- [ ] Logo (hoje aparece "SUA LOGO" no nav e footer)
- [ ] Número de WhatsApp — `5511900000000` (várias ocorrências)
- [ ] Dados de contato, endereço e mapa (seção Localização)
- [ ] Números fictícios (4.800 aprovados, 15 anos, 94%)
- [ ] Depoimentos (são exemplos)
- [ ] URLs de SEO no `<head>`: `vialivre.com.br` e `preview.jpg`
- [ ] Imagem de preview Open Graph (1200×630)
- [ ] Links de redes sociais (`/suaautoescola`)

---

## Pontos de restauração (git tags)

| Tag | O que é |
|-----|---------|
| `checkpoint-estavel` | Versão estável aprovada: categorias 3×2, como funciona, animações suaves, menu mobile ok (antes do SEO/FAQ) |

**Voltar para um checkpoint:**

```bash
cd site-demonstracao
git reset --hard checkpoint-estavel
git push --force origin main
```

---

## Histórico de melhorias

- Seção "Como funciona" (3 passos)
- Correção do menu hambúrguer mobile
- Animações de scroll mais suaves e escalonadas
- Grid de categorias organizado (3×2 no desktop) + badges nos ícones
- SEO completo + Open Graph + seção de FAQ + dados estruturados
