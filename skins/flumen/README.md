# Skin Flumen (Roundcube) - Clara frontend

Pack listo para deploy en el Roundcube de webmail.flumen.com.ar.
Extiende Elastic. Login: casilla + password. Sin textos de anotador (ley 22).

## Path en repo
Agentes/projects/flumenroundcube/skins/flumen/

## Deploy (Nora / Gregory)
1. Copiar carpeta `flumen` a `{roundcube}/skins/flumen/`
2. En config.inc.php (o local):
   - $config['skin'] = 'flumen';
   - $config['product_name'] = 'Flumen Webmail';
   - $config['display_product_info'] = 0;
   - $config['imap_host'] = 'ssl://mail.postale.io:993';
   - $config['smtp_host'] = 'ssl://mail.postale.io:465';
3. Con imap_host string fijo, Roundcube no muestra campo Servidor.
   La skin tambien oculta #rcmloginhost por CSS/JS por si queda visible.
4. No tocar apex flumen.com.ar ni MX Postale.

## Contenido
- meta.json (extends elastic + stylesheet flumen.css)
- styles/flumen.css (colores marca)
- templates/login.html (logo Flumen, footer publico limpio)
- images/ logo.svg + png + favicon

## Colores
- Deep #071A2B / River #0F7B9E / Current #22C3E6 / Sand #F2A541
