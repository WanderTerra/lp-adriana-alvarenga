# Dúvidas para alinhar com a cliente (Dra. Adriana)

Perguntas em aberto que dependem de informação/decisão dela antes de fechar a página.

## 1. SEO / estratégia de tráfego

Confirmado: a trava do vídeo (conteúdo só libera depois de assistir/pular) **fica como está** — foi pedido explicitamente pela cliente.

Isso tem uma consequência técnica: como o Google não clica em "assistir", ele não vê quase nenhum texto da página hoje (só o masthead e o título/lead antes do vídeo — todo o resto, ~90% do conteúdo, só aparece via JS depois de interação). Isso é normal e aceitável para páginas de VSL (vídeo de vendas) que rodam só em tráfego pago (Meta Ads, Google Ads).

**Perguntar para a cliente:** além do tráfego pago, ela espera/quer que essa página apareça em buscas do Google (SEO orgânico)?

- Se **não** → tudo certo, não precisa mexer em mais nada além do que já foi feito (meta description, Open Graph).
- Se **sim** → existe uma forma de resolver sem tirar a trava visual (trocar "revelar por clique" por "revelar por timer automático" ao carregar a página), mas é um ajuste técnico adicional que precisa ser combinado, já que muda o comportamento de quando o conteúdo é liberado.

## 2. Domínio / publicação

Para terminar o SEO básico da página falta:
- **Qual vai ser a URL final** (domínio) onde a página vai ficar publicada — necessário para preencher `canonical` e `og:url` no `<head>`.
- **Uma imagem de preview** (para `og:image`, o card que aparece quando o link é compartilhado no WhatsApp/Instagram/Facebook). Precisa ser um arquivo hospedado com URL pública — não dá pra usar a logo embutida em base64 que está no código hoje.

## 3. Garantia

O MD de copy pede um bloco "Garantia de (X dias)" que já foi adicionado na seção de oferta, mas **o prazo de dias ainda está com placeholder** (`[X]` dias) — marcado com comentário `TODO` no código.

**Perguntar para a cliente:** quantos dias de garantia ela quer oferecer?

## 4. Preço

Os valores usados na seção de oferta hoje foram mantidos do site original (De R$ 2.997 → 12x R$149 no cartão ou R$1.497 à vista), já que o MD de copy deixava o preço em aberto ("ENTRA O PREÇO"). **Confirmar se esses valores continuam corretos** ou se ela quer atualizar.

## 5. Materiais pendentes (já sabidos, só reforçando)

- Vídeo real (hoje é uma simulação)
- Fotos/prints/depoimentos de pacientes (seção 11 do MD)
- Foto profissional da Dra. Adriana (seção "Quem será sua mentora")
