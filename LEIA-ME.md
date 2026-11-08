# Repositório raiz — despertadoativo-blip.github.io

Este repositório existe só para o Android confirmar que o site do AquaGest Pro é seu (Digital Asset Links).
Sem ele, o app da Play Store abre com a barra de endereço do navegador.

## Como criar
1. No GitHub, crie um repositório público com o nome exato **despertadoativo-blip.github.io**.
2. Envie os arquivos desta pasta: `.nojekyll`, `index.html` e a pasta `.well-known` com `assetlinks.json`.
   - O `.nojekyll` é obrigatório: sem ele o GitHub Pages não publica pastas que começam com ponto.
3. Em Settings › Pages, publique a partir do ramo `main`, pasta `/ (root)`.

## Os dois códigos SHA-256 do assetlinks.json
- **Chave de upload:** vem no arquivo `signing-key-info.txt` do pacote baixado do PWABuilder (linha SHA-256).
- **Chave de assinatura do app:** no Play Console, abra o app › Versão › Configuração › Integridade do app ›
  "Certificado da chave de assinatura do app" › SHA-256.
- Troque os dois textos COLE_AQUI… pelos códigos (formato `AA:BB:CC:…`, com dois-pontos).

## Conferir
Abra https://despertadoativo-blip.github.io/.well-known/assetlinks.json — o arquivo tem de aparecer.
Teste oficial do Google (troque nada, só abra):
https://digitalassetlinks.googleapis.com/v1/statements:list?source.web.site=https://despertadoativo-blip.github.io&relation=delegate_permission/common.handle_all_urls
