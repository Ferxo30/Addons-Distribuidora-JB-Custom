# Normalización de nombres técnicos

Desde el segundo commit del repositorio, todos los addons terminan en `_ferre`.

> **Importante:** estos ocho cambios alteran el nombre técnico del módulo Odoo. No se deben copiar sobre una base que tenga instalados los nombres anteriores sin ejecutar una migración controlada de `ir.module.module`, XML IDs y referencias relacionadas. Este commit solo normaliza el repositorio; no modifica FERRE_PROD, FERRE_TEST ni FERRE_UAT.

| Nombre anterior en UAT | Nombre normalizado en Git |
|---|---|
| `ferreteria_fel_nc_annul_qa_fix` | `ferreteria_fel_nc_annul_qa_fix_ferre` |
| `ferreteria_pos_fel_ticket` | `ferreteria_pos_fel_ticket_ferre` |
| `l10n_gt_check_printing2` | `l10n_gt_check_printing2_ferre` |
| `l10n_gt_check_printing2_voucher` | `l10n_gt_check_printing2_voucher_ferre` |
| `partner_supplier_code_v1` | `partner_supplier_code_v1_ferre` |
| `pos_receipt_hide_prices` | `pos_receipt_hide_prices_ferre` |
| `pos_report_generator` | `pos_report_generator_ferre` |
| `stock_scrap_print_button_fix` | `stock_scrap_print_button_fix_ferre` |
