# EShoppingZone Cloud Config Repository

This folder contains the centralized configuration properties for all microservices in the EShoppingZone project.

## How to push these files to your GitHub Repository

Run the following commands in PowerShell from inside this `cloud-config-repo` directory:

```bash
cd "C:\Users\user\Documents\abulEshopping\cloud-config-repo"
git init
git add .
git commit -m "Add centralized configuration for all EShoppingZone microservices"
git branch -M main
git remote add origin https://github.com/Abulhasan06/Eshopping-cloudconfig-server.git
git push -u origin main --force
```

## Files included:
- `application.properties` (Global shared configuration, Eureka URL, Actuator endpoints)
- `api-gateway.properties` (Routing definitions for all services)
- `auth-service.properties` (Port 8081, Auth DB, JWT token settings)
- `profile-service.properties` (Port 8082, Profile DB)
- `product-service.properties` (Port 8083, Product DB)
- `cart-service.properties` (Port 8084, Cart DB)
- `order-service.properties` (Port 8085, Order DB)
- `payment-service.properties` (Port 8086, Payment DB, 90/10 split settings)
- `delivery-service.properties` (Port 8087, Delivery DB)
- `notification-service.properties` (Port 8088, Notification DB, SMTP Mail)
- `wallet-service.properties` (Port 8089, Wallet DB)
- `website-controller.properties` (Port 8090, UI, Gateway service URLs)
