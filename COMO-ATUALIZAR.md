# Como atualizar a página de links da Lia

Endereço: **https://lianacostura.github.io**
Pasta no computador: `Área de Trabalho\lia-links` (separada da Vênus de propósito)
Repositório: https://github.com/lianacostura/lianacostura.github.io

## Jeito mais fácil
Gere o link no painel de afiliados da Shopee (conta venus.bordado, que é a do CPF) em
Ofertas → Ofertas de produtos → "Obter link", e mande pro Claude:
"acrescenta na página da Lia: https://s.shopee.com.br/... (calcador de zíper)".
Ele confere o anúncio, coloca a foto e publica.

## Na mão
1. Foto quadrada (600 px, .webp) solta na pasta, sem subpasta (o envio pelo site do GitHub não aceita subpasta).
2. Em `dados.json`, um bloco por produto:
   ```json
   { "nome": "Agulha para jeans 100/16", "nota": "A que salvou a calça da Dona Cida",
     "foto": "agulha-jeans.webp", "link": "https://s.shopee.com.br/...",
     "categoria": "Agulhas e calcadores", "data": "2026-11-09", "destaque": false }
   ```
   `nota` e `destaque` são opcionais (destaque = aparece primeiro, ex.: a overloque).
3. Publicar: em https://github.com/lianacostura/lianacostura.github.io/upload/main (logada na conta
   GitHub da Lia, lianacosturaoficial-spec), enviar `dados.json` + a foto nova e clicar em "Commit changes".
   (A conta GitHub da Vênus não tem acesso a esta organização: git push daqui não funciona.)

## Categorias
Máquinas · Agulhas e calcadores · Corte e medida · Linhas e aviamentos
(mais de 6 produtos: os filtros aparecem sozinhos)

## Regras (não quebrar)
- Nome, foto e link do MESMO anúncio.
- Nada de preço, nota, "mais vendido" ou promoção que o anúncio não mostre.
- Só link de afiliado do painel. Nunca produto da Vênus aqui.
- A `nota` pode ligar o produto à história ("a agulha que quebrou no cós"), sem dizer que a Lia
  é uma pessoa real usando o produto.

## Produtos no ar (09/11/2026)
Overloque Singer 1300 (destaque) · agulha Singer 100/16 jeans · kit 42 calcadores · tesoura de alfaiate 24 cm · 2 fitas métricas · abridor de casas (2) · alfineteiro magnético · 10 retrós coloridos. Links gerados pelo Claude com Chrome no painel da conta venus.bordado; fotos = imagem do anúncio na Shopee.
