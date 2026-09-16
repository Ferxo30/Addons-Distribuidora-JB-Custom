# Addons Distribuidora JB Custom

Repositorio maestro de addons personalizados para:

**DISTRIBUIDORA Y FERRETERÍA JB, S.A.**

Plataforma base: **Odoo 18.0-20250520 Community**.

## Propósito

Este repositorio contiene los addons personalizados utilizados por la implementación Odoo de Distribuidora y Ferretería JB. La rama `main` representa la línea consolidada del proyecto.

La versión inicial se obtuvo de las copias efectivamente cargadas y validadas en el runtime `FERRE_UAT`. El detalle de módulos, versiones y huellas de integridad se encuentra en [MANIFIESTO_MODULOS.md](MANIFIESTO_MODULOS.md).

## Convención de nombres

Los 57 addons del repositorio terminan en `_ferre`.

Ocho módulos recibieron este sufijo después de la importación inicial. Como el nombre de carpeta es el nombre técnico de un módulo Odoo, esos cambios no deben desplegarse directamente sobre una base que todavía tenga instalados los nombres anteriores. El mapeo y la advertencia de migración están en [RENOMBRES_MODULOS.md](RENOMBRES_MODULOS.md).

## Alcance

- Código fuente de 57 addons personalizados.
- No incluye módulos estándar de Odoo.
- No incluye bases de datos, filestore, respaldos, logs, inventarios ni datos empresariales exportados.
- No incluye archivos de configuración local, contraseñas, tokens, credenciales FEL/Megaprint, SMTP o PostgreSQL.

Las credenciales y configuraciones operativas deben almacenarse en Odoo o en mecanismos seguros del ambiente de despliegue, nunca en el repositorio.

## Estructura

```text
Addons-Distribuidora-JB-Custom/
├── README.md
├── .gitignore
├── MANIFIESTO_MODULOS.md
├── RENOMBRES_MODULOS.md
└── addons/
    └── <57 módulos personalizados con sufijo _ferre>
```

## Despliegue

Los addons deben instalarse en una ruta separada de los addons estándar e incluirse explícitamente en `addons_path`. Antes de actualizar módulos se deben revisar versiones, dependencias y diferencias respecto del ambiente objetivo.

Para los ocho módulos renombrados, primero debe diseñarse y probarse una migración técnica en una copia de la base. Renombrar una carpeta no migra automáticamente `ir.module.module`, XML IDs ni datos ya instalados.
