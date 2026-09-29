# Branding Flumen sobre Elastic (MSG 019)

correo.flumen.com.ar mantiene skin **elastic** (layout stock).
Branding = logos + favicon + product_name Flumen. NO activar skin flumen full.

## Assets (FTP)
Subir carpeta completa:
`projects/flumenroundcube/skins/flumen/images/`
hacia:
`{roundcube_custom}/skins/flumen/images/`

Archivos:
- logo.svg, logo-dark.svg
- logo-small.svg, logo-small-dark.svg, logo-small.png, logo.png
- favicon.ico, favicon.png, favicon.svg

No hace falta templates ni meta de skin flumen. Solo images (+ snippet en config).

## Config
Aplicar `config-snippet.php.txt` al config del install custom:
- skin=elastic
- product_name=Flumen Webmail
- skin_logo + favicon apuntando a skins/flumen/images/*

## Checklist Admin/Gregory
1. Login: logo Flumen, layout elastic centrado
2. Inbox/header: logo small / dark segun modo
3. Favicon Flumen en pestana
4. Titulos / about: Flumen Webmail (sin Roundcube generico donde config alcanza)
5. IMAP/SMTP Postale intactos; NO Hestia webmail; cutover hold

## Paths repo
- Primary: projects/flumenroundcube/skins/flumen/
- Mirror: projects/flumenroundcube/roundcubemail/skins/flumen/
