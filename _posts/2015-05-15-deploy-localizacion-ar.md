---
layout: post
title: "Deploy entorno localización Argentina"
modified: 2015-05-15 14:44:38 -0300
category: []
tags: [reunion, home, deploy, pypi, localizacion]
image:
  feature: 
  credit: 
  creditlink: 
comments: 
share: 
---

Creamos un [script de deploy](https://github.com/tryton-ar/deploy-localizacion-argentina) para deployar un entorno de Tryton 3.4 con la localización de Argentina (AFIP, voucher, Factura Electrónica, etc). El script genera un virtualenv, te instala todos los requerimientos usando pip, y te genera un scenario base con todas las parametrizaciones. La base de datos que genera se va a terminar llamando *tryton_ar_3_4*.

Obviamente, se deben instalar los requerimientos (postgresql, etc) previamente. Por favor, leer el README para más información

Lo único, es que por el momento esta basado en 3.4, ya que los módulos de localización argentina únicamente están para 3.4
Para facilitar la instalación, subimos los módulos de Tryton-Ar a pypi.

Si alguno quiere contribuir con su módulo, lo que les pedimos es que el prefijo sean *trytonar* para que de esa manera, buscarlo con pypi sea facil.

~ ❯❯❯ pip search trytonar
```
trytonar_account_invoice_ar - Localizacion para Argentina. Integración AFIP, Factura Electronica
trytonar_account_check_ar - Tryton module for accounting check of Argentina
trytonar_account_bank_ar  - Tryton module with banks of Argentina
trytonar_account_ar       - Tryton module to add an account chart template for Argentina
trytonar_account_voucher_ar - Tryton module to add payments and receipts for Argentina
trytonar_account_coop_ar  - Tryton module to add an account chart template for Cooperative Argentina
trytonar_account_retencion_ar - Tryton module with accounting withholding for Argentina
```
