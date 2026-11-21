# Plano técnico de descoberta — PITOMBA ATÔMICA LAB

Base: GitHub Pages, URL pública atual em subdiretório. Idioma/mercado inicial: português do Brasil; vendas inicialmente no Brasil. Revisão: 21/11/2026.

## Princípios
- SEO técnico e conteúdo útil são a base de descoberta em buscadores tradicionais e recursos generativos.
- GEO não é um conjunto de hacks nem garantia de citações. Google declara que não exige arquivos especiais ou marcação exclusiva para recursos de IA; páginas precisam ser indexáveis e úteis.
- Conteúdo estruturado deve corresponder ao que o visitante realmente vê.
- Não usar avaliações, preços, estoque, endereço físico, certificações ou alegações de sustentabilidade sem comprovação.

## Estado técnico implementado
- Metadados básicos, canonical, Open Graph e Twitter summary no HTML inicial.
- JSON-LD Organization e WebSite.
- robots.txt com OAI-SearchBot permitido e GPTBot bloqueado; são controles independentes.
- Sitemap XML inicial com a página inicial.
- Favicon SVG.

## Limitações atuais
- O site ainda está hospedado em github.io; domínio próprio é recomendável antes de escalar marca e backlinks.
- Só existe uma URL pública de conteúdo. As coleções não possuem páginas próprias e não há fichas de obra indexáveis.
- Não há imagens sociais raster (Open Graph 1200×630), galeria real, dados de produto, checkout, política de frete/devolução, contato confirmado ou captura de leads.
- Não existe negócio local com endereço público confirmado. Não implementar LocalBusiness nem inventar presença física/Google Business Profile.
- Sitemap será expandido quando houver URLs reais e estáveis.

## Arquitetura alvo
1. / — marca, proposta, navegação para coleções.
2. /colecoes/ — índice editorial das coleções.
3. /colecoes/nome-da-colecao/ — página independente, texto original, curadoria e links para obras.
4. /obras/slug-da-obra/ — ficha individual: título, artista/marca, descrição, dimensões, técnica, suporte, opções, preço real, disponibilidade, prazo e envio quando confirmados.
5. /sobre/ — história institucional da marca, processo editorial e critérios de produção; sem expor dados pessoais não autorizados.
6. /faq/, /contato/, /envio-e-devolucao/, /privacidade/ — publicar quando as regras operacionais estiverem definidas.

## SEO técnico — checklist
- [ ] Confirmar propriedade no Google Search Console por método DNS/HTML compatível com GitHub Pages.
- [ ] Enviar sitemap.xml ao Search Console.
- [ ] Configurar Bing Webmaster Tools e importar/verificar sitemap.
- [ ] Verificar rastreamento e indexação de URLs prioritárias.
- [ ] Validar HTML, canonical, títulos, descrições, headings, links internos, status HTTP e mobile.
- [ ] Adicionar imagem OG 1200×630 em PNG/JPG e imagens de obra em WebP/AVIF com fallback.
- [ ] Implementar ImageObject/Product somente nas fichas com conteúdo e dados comerciais reais.
- [ ] Monitorar Core Web Vitals, acessibilidade, peso de imagens e dependência de fontes externas.
- [ ] Considerar domínio próprio e redirecionamento canônico antes de acumular backlinks.

## GEO / busca por IA
- [ ] Permitir OAI-SearchBot se a prioridade for aparecer na busca do ChatGPT.
- [ ] Decisão separada sobre GPTBot: bloqueado nesta configuração para não autorizar rastreamento voltado a treinamento; rever se a política de licenciamento mudar.
- [ ] Manter páginas com definições claras, autoria institucional, fatos verificáveis, texto visível e links internos.
- [ ] Publicar conteúdo editorial original: processos, materiais, dimensões, critérios de curadoria e guias de composição, sem produzir páginas genéricas em escala.
- [ ] Monitorar citações/visibilidade em ChatGPT, Gemini, Perplexity e Copilot manualmente; não prometer ranking nem citação.
- [ ] Não tratar llms.txt como requisito de Google ou garantia de indexação/citação.

## SEO de imagens e descoberta visual
- [ ] Nomear arquivos de forma descritiva e estável.
- [ ] Alt text descreve o que a imagem mostra; não empilhar palavras-chave.
- [ ] Legendas com título, coleção, técnica e dimensões quando verdadeiros.
- [ ] Imagens originais em alta resolução; miniaturas e versões responsivas.
- [ ] Pinterest: perfil de marca, pins individuais que apontem para a página da obra, metadados OG e consistência de destino.

## Comércio e confiança — antes de vender
- [ ] Homologar fornecedor com amostras físicas e custo total por região.
- [ ] Definir preços, margem, prazos, embalagem, reimpressão, avaria e atendimento.
- [ ] Criar fichas de obra e páginas legais coerentes com operação real.
- [ ] Só então adicionar schema Product/Offer, feed de produtos e integração com Merchant Center, se elegível.
- [ ] Implementar checkout e analytics de conversão com consentimento e política de privacidade adequados.

## Métricas
- Indexação: páginas válidas, excluídas e erros de rastreamento.
- Descoberta: impressões, cliques, CTR e consultas no Search Console/Bing.
- Conteúdo: entradas orgânicas por URL, imagens exibidas e tráfego Pinterest.
- Negócio: cliques em CTA, contatos qualificados, adição ao carrinho, conversão, margem por obra e devoluções.
- GEO: referências/citações observadas e sessões atribuídas a mecanismos generativos, quando analytics permitir identificar origem.

## Fontes oficiais consultadas
- Google Search Central — AI features: https://developers.google.com/search/docs/appearance/ai-features
- Google Search Central — controle de rastreamento e recursos de IA: https://developers.google.com/search/docs/crawling-indexing/control-what-you-share
- Bing Webmaster Guidelines: https://www.bing.com/webmasters/help/webmaster-guidelines-30fba23a
- Bing IndexNow: https://www.bing.com/webmasters/help/indexnow-0z209wby
- OpenAI crawler documentation: https://developers.openai.com/api/docs/bots

Status: base técnica inicial implementada; arquitetura editorial, conteúdo, domínio próprio, analytics e integrações de comércio permanecem pendentes.
