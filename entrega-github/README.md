# Conciliacao financeira dpen

Site de arquivo unico (`index.html`) que le as planilhas no navegador e concilia o dashboard com Cielo, PagBank e Safra. Nada e enviado a servidor.

## Regras
- **Nunca** subir planilhas reais neste repositorio (o `.gitignore` bloqueia xlsx/csv). Este repositorio deve ser **privado**.
- Para atualizar o site: substituir o `index.html` e fazer commit. O deploy na Hostinger pega a nova versao.

## Publicar na Hostinger (Git)
hPanel > Avancado > Git > repositorio deste GitHub, branch `main`, pasta de destino `public_html` (ou a pasta do subdominio) > Implantar.
Depois: SSL ativo e **Pastas protegidas por senha** na pasta do site.

## Arquivos
- `index.html` - o site
- `.htaccess` - HTTPS, cabecalhos de seguranca, sem cache de HTML, bloqueia README
- `robots.txt` - pede aos buscadores para nao indexar
- `.gitignore` - impede subir dados reais