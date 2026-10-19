# Restaurant Management

A browser-based restaurant operations demo with a dark, glass-inspired interface. This is the first product in a planned family of tools; Quick Service Management may be added later as a separate experience on shared concepts.

## Current demo

- Overview dashboard with revenue, order, occupancy, activity and popular-item summaries
- Orders: search, status filtering, create order, advance order status
- Floor & tables: table availability, seating and status changes
- Menu: create/edit products, categories, prices, descriptions, emoji and availability
- Inventory: ingredient quantities, minimum stock alerts, stock adjustments
- Staff: team roster and shift/status editing
- Reports: category sales snapshot and data export
- Settings: restaurant/branch name, currency, tax rate and hours
- JSON export of locally saved data
- Responsive layout for desktop and mobile

## Run locally

Open `index.html` in a modern browser. No build step or server is required for this demo.

## Persistence and limitations

The app stores demo data in browser `localStorage` under `restaurant-management-demo-v1`. Data remains in the same browser profile on the same device. It is not shared across staff, browsers, devices or branches, and clearing site data can remove it. Do not enter sensitive customer data.

This is a prototype, not a production POS or multi-tenant SaaS. Authentication, server-side validation, shared database persistence, audit logging, payments, backups, permissions, and production security are not implemented.

## Architecture direction

Keep restaurant configuration and catalog concepts reusable so a future Quick Service Management experience can add counter/pickup flows, combos/modifiers, kitchen display and queue-time metrics without duplicating the entire foundation.

## Repository

https://github.com/appenzellerdigitalstore-stack/restaurant-management
