# Awesome-Order-Processing-Fulfillment

# Awesome Order Processing & Fulfillment

> A curated list of top Order Processing and Fulfillment platforms — both SaaS/Hosted commercial solutions and open-source alternatives for managing orders, inventory, shipping, and warehouse operations.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [ShipStation](#shipstation)
  - [ShipBob](#shipbob)
  - [Brightpearl](#brightpearl)
  - [Cin7](#cin7)
  - [Skubana](#skubana)
- [Open-Source Software](#-open-source-software)
  - [OpenOMS](#openoms)
  - [KubeRiva OMS](#kuberiva-oms)
  - [ModernWMS](#modernwms)
  - [Sentry WMS](#sentry-wms)
  - [OpenBoxes](#openboxes)
  - [OverSeek](#overseek)
  - [Fleetbase](#fleetbase)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Order Processing and Fulfillment platforms. These are not open-source but are included as reference points for feature comparison.

### ShipStation
**Type:** Multi-channel shipping and order fulfillment  
ShipStation is one of the most widely adopted shipping platforms, connecting e-commerce channels, carriers, and warehouses to streamline order fulfillment. It supports automated order import, batch shipping, label printing, and tracking across major carriers.

### ShipBob
**Type:** Third-party logistics (3PL) with fulfillment network  
ShipBob provides outsourced fulfillment through its network of warehouses, handling storage, picking, packing, and shipping for e-commerce brands. It integrates with major sales channels and offers real-time inventory visibility.

### Brightpearl
**Type:** Retail operations platform with order and inventory management  
Brightpearl combines inventory, orders, warehouses, accounting, and fulfillment in a centralized system, positioned for multichannel retailers with high order volume.

### Cin7
**Type:** Inventory-centric fulfillment with deep e-commerce integrations  
Cin7 combines inventory management with order routing, warehouse workflows, and POS, supporting 450+ integrations including Shopify, Amazon, and QuickBooks.

### Skubana
**Type:** Order management and inventory for high-volume sellers  
Skubana provides order management, inventory, and analytics for e-commerce sellers, with multi-channel support and demand forecasting.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Order Processing and Fulfillment tools. The open-source ecosystem spans **AI-native OMS platforms**, **warehouse management systems**, and **e-commerce operations hubs**.

### OpenOMS
**Stack:** Go / TypeScript / PostgreSQL / Redis | **License:** ELv2 (API/Dashboard) / MIT (SDK packages)  
OpenOMS is an open-source Order Management System for e-commerce, with **345 Go source files, 308 TypeScript files, 463 API endpoints, and 141 dashboard pages** [citation:3]. It includes **27 standalone SDK packages** (MIT-licensed) for integrations like Allegro, and a Helm chart for Kubernetes deployment. The codebase is actively developed with a full CI pipeline. **Note:** The API server and dashboard are under the Elastic License 2.0 (ELv2), while SDK packages are MIT [citation:3].  
**Best for:** E-commerce businesses wanting a comprehensive, self-hosted OMS with broad integration support and a mature Go/TypeScript stack.

### KubeRiva OMS
**Stack:** FastAPI / Python / PostgreSQL / MongoDB / Redis / Elasticsearch | **License:** Open Source (AI-native OMS)  
KubeRiva OMS is an open-source **AI-native OMS** positioned as a self-hosted alternative to enterprise SaaS costing $200k/year [citation:1]. Key features include:
- **7 intelligent sourcing strategies** with AI node scoring and NL-to-proposals
- **Fulfillment nodes** with capability flags (ship/pickup/curbside/same-day), daily capacity, and geo-based sourcing distance calculations
- **15-state order machine** covering WEB, MOBILE, POS, API, and MARKETPLACE channels
- **Docker Compose** deployment of all 8 services in one command
- **LLM-agnostic** AI layer (default: Claude Haiku)

The architecture uses PostgreSQL 16 for primary data, MongoDB 7 for event logs, Redis 7.2 for caching/queues, and Elasticsearch 8.12 for search [citation:1].  
**Best for:** E-commerce and retail businesses wanting an AI-driven, self-hosted OMS with intelligent sourcing and multi-channel order management.

### ModernWMS
**Stack:** (Check repository) | **License:** Open Source  
ModernWMS is an open-source warehouse management system derived from years of ERP implementation experience, described as "simple and complete" and stripped from a commercial system to help small and medium-sized enterprises [citation:2]. It supports cross-platform operation and has **2k GitHub stars and 479 forks** [citation:2].  
**Best for:** SMEs wanting a proven, straightforward WMS with a solid community following.

### Sentry WMS
**Stack:** (Check repository) | **License:** Open Source  
Sentry WMS is an open-source warehouse management system for e-commerce, with a comprehensive API covering **receiving, put-away, picking, packing, shipping, cycle counting, bin transfers, inventory adjustments, and inter-warehouse transfers** [citation:4]. It supports wave picking, batch creation with optimized walk paths, barcode validation, and short-pick reporting. The API is well-documented with clear endpoints for each warehouse operation [citation:4].  
**Best for:** E-commerce warehouses needing a structured WMS with granular API control over every fulfillment step.

### OpenBoxes
**Stack:** Groovy / Grails | **License:** EPL-1.0  
OpenBoxes is a warehouse management system designed for **healthcare facilities**, managing inventory and tracking stock movements for medical supplies [citation:6]. It has **920 stars, 511 forks**, and active development (last push October 2026). It is used in disaster response and healthcare supply chain contexts [citation:6].  
**Best for:** Healthcare organizations and NGOs needing inventory and shipment tracking tailored to medical supplies.

### OverSeek
**Stack:** Node.js / PostgreSQL / Elasticsearch / Redis | **License:** Open Source  
OverSeek is a self-hosted **e-commerce operations hub for WooCommerce**, unifying orders, inventory, shipping, customers, analytics, and marketing in one private workspace [citation:8]. Features include WooCommerce order sync with fulfillment context, shipment tracking with carrier links, inventory/supply chain management, purchase orders, supplier context, and a mobile PWA. It deploys via Docker Compose and includes an MCP server and CLI package [citation:8].  
**Best for:** WooCommerce store owners wanting a self-hosted operations dashboard that consolidates order and fulfillment management.

### Fleetbase
**Stack:** JavaScript / PHP | **License:** AGPL-3.0  
Fleetbase is a modular **logistics and supply chain operating system (LSOS)** with 4,427 GitHub stars and active development [citation:11]. It includes a **WooCommerce plugin for last-mile delivery** with live delivery quotes, driver/vehicle management, automatic order sync, and status back to WooCommerce with no per-delivery fees [citation:11]. It also offers storefront and marketplace extensions, making it a comprehensive logistics platform.  
**Best for:** Businesses needing last-mile delivery orchestration integrated with WooCommerce, with broader logistics management capabilities.

---

## 📊 Comparison at a Glance

| Software | License | Stack | OMS Focus | WMS Focus | Self-Hosted | Best For |
|----------|---------|-------|-----------|-----------|-------------|----------|
| **OpenOMS** | ELv2 / MIT | Go/TS/Postgres | ✅ | (Check) | ✅ | Full e-commerce OMS |
| **KubeRiva OMS** | Open Source | Python/Postgres | ✅ AI-native | (Check) | ✅ | AI sourcing + multi-channel |
| **ModernWMS** | Open Source | (Check) | ❌ | ✅ | ✅ | SME warehouse management |
| **Sentry WMS** | Open Source | (Check) | (Check) | ✅ Granular API | ✅ | E-commerce warehouse ops |
| **OpenBoxes** | EPL-1.0 | Groovy/Grails | ❌ | ✅ Healthcare | ✅ | Medical supply tracking |
| **OverSeek** | Open Source | Node.js/Postgres | ✅ WooCommerce | ✅ Inventory | ✅ | WooCommerce ops hub |
| **Fleetbase** | AGPL-3.0 | JS/PHP | ✅ Delivery | (Check) | ✅ | Last-mile delivery |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Order Processing or Fulfillment tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** Order processing and fulfillment splits between **full OMS platforms** (OpenOMS for broad e-commerce, KubeRiva for AI-native sourcing) and **warehouse management systems** (ModernWMS for SMEs, Sentry WMS for granular API control, OpenBoxes for healthcare). **OverSeek** uniquely targets WooCommerce stores with a self-hosted operations hub, while **Fleetbase** focuses on last-mile delivery orchestration. No single open-source project replicates the full breadth of ShipStation or ShipBob, but combinations of OMS + WMS can cover most fulfillment workflows.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
