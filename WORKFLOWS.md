# ops — n8n Automation Workflows

Production automation workflows built for small-business operations (inventory, purchasing, fulfilment, lead handling). Built in [n8n](https://n8n.io), orchestrating Google Sheets, Gmail, Slack and external APIs.

Each `.json` here is an importable n8n workflow export. Captured execution data and credential IDs have been removed; workflows reference credentials by name only.

## Workflows

### Ops Webhook
- **File:** `ops_Webhook.json`  
- **Nodes:** 2 — webhook, Google Sheets

### Low-Stock Reorder Alerts (v4 - PO writer)
- **File:** `Low_Stock_Reorder_Alerts_v4_PO_writer_.json`  
- **Nodes:** 10 — Google Sheets ×5, code ×2, schedule, merge, Slack

### Customer Shipment Notifications (v2 - split aware)
- **File:** `Customer_Shipment_Notifications_v2_split_aware_.json`  
- **Nodes:** 6 — Google Sheets ×2, Sheets trigger, code, if, Gmail


### Inbound Email Triage (Gmail + Claude)
- **File:** `Inbound_Email_Triage_Gmail_Claude_.json`  
- **Nodes:** 19 — Gmail ×11, Slack ×3, Gmail trigger, set, HTTP/API, code, switch

### Low-Stock Reorder Alerts
- **File:** `Low_Stock_Reorder_Alerts.json`  
- **Nodes:** 6 — Google Sheets ×2, schedule, merge, code, Slack

### PurchaseOrders Lifecycle (v2 - firm-date email)
- **File:** `PurchaseOrders_Lifecycle_v2_firm_date_email_.json`  
- **Nodes:** 9 — Google Sheets ×4, code ×3, schedule, Gmail

### Duomenu tvarkymas - Stock and Leads
- **File:** `Duomenu_tvarkymas_Stock_and_Leads.json`  
- **Nodes:** 9 — Google Sheets ×4, code ×4, manual

### Supplier Doc Extractor (v2 - CleanLeads enrich)
- **File:** `Supplier_Doc_Extractor_v2_CleanLeads_enrich_.json`  
- **Nodes:** 8 — code ×3, Google Sheets ×2, form, file extract, HTTP/API

### Warehouse Automation (v5 - backorder split)
- **File:** `Warehouse_Automation_v5_backorder_split_.json`  
- **Nodes:** 11 — Google Sheets ×6, code ×3, form, merge
