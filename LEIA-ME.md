# Estúdio Vibe Barbearia — Landing page

Site estático (HTML + CSS inline + ~1 KB de JS). Sem build. Basta subir a pasta `site/` para qualquer hospedagem (Vercel, Netlify, Hostinger, Cloudflare Pages).

## Antes de publicar — preencher (busque por `EDITAR` no index.html)

| Item | Onde |
|---|---|
| Domínio definitivo (hoje `devprodigio.github.io/studio-vibe-barbearia`) | `index.html` (canonical, og:url, og:image, JSON-LD), `robots.txt`, `sitemap.xml` |
| Endereço completo (rua, nº, bairro) | seção Localização + `address` no JSON-LD (`streetAddress`) |
| Coordenadas exatas da barbearia | `geo.position`, `ICBM` e `geo` no JSON-LD (hoje: centro de LEM) |
| Telefone / WhatsApp | adicionar `telephone` no JSON-LD e um botão `https://wa.me/55DDDNUMERO` |
| Horário de funcionamento | seção Localização + `openingHoursSpecification` no JSON-LD |
| Fotos reais (cortes, ambiente, equipe) | recomendado incluir uma galeria — aumenta muito a conversão |

## SEO local — checklist pós-publicação
1. Google Search Console: verificar domínio e enviar `sitemap.xml`.
2. Google Business Profile: categoria principal **Barbearia**, mesmo nome/endereço/telefone (NAP) do site, link do site + link de agendamento.
3. Pedir avaliações no Google aos clientes (maior fator de ranqueamento no Maps).
4. Link do site na bio do Instagram.
5. Validar dados estruturados: https://search.google.com/test/rich-results

## Conversão
Todos os botões têm `data-cta`. Se GA4 (`gtag`) ou Meta Pixel (`fbq`) forem instalados, os cliques disparam `agendar_click` / `Schedule` automaticamente.
