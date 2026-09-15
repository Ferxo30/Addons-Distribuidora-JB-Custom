# Addons Distribuidora JB Custom

Repositorio maestro de addons personalizados para:

**DISTRIBUIDORA Y FERRETERÍA JB, S.A.**

Plataforma base: **Odoo 18.0-20250520 Community**.

## Propósito

Este repositorio contiene los addons personalizados utilizados por la implementación Odoo de Distribuidora y Ferretería JB. La rama `main` representa la línea consolidada del proyecto.

La versión inicial se obtuvo de las copias efectivamente cargadas y validadas en el runtime `FERRE_UAT`. El detalle de módulos, versiones y huellas de integridad se encuentra en [MANIFIESTO_MODULOS.md](MANIFIESTO_MODULOS.md).

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
└── addons/
    └── <57 módulos personalizados>
```

## Despliegue

Los addons deben instalarse en una ruta separada de los addons estándar e incluirse explícitamente en `addons_path`. Antes de actualizar módulos se deben revisar versiones, dependencias y diferencias respecto del ambiente objetivo.

