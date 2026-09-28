# storefront

The four services behind the shop.

| Service | Path | Owner |
|---|---|---|
| `shop-web` | `services/web` | Web |
| `shop-checkout` | `services/checkout` | Payments |
| `shop-payments` | `services/payments` | Payments |
| `shop-catalog` | `services/catalog` | Catalog |

All four build from the root `Dockerfile`. `SERVICE_MODULE` picks the app,
`SERVICE_NAME` sets the telemetry service name.

Payment authorisation is handled by our PSP, which is external and which we
do not instrument.
