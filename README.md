## Introduction
---
  
The JTM Network was made to host personal projects that solve business problems. Using microservice architecture I can add features to my website without affecting the other services, and provides scalability when necessary.

## Tech Stack
---

### Languages
- HTML, CSS, Javascript
- Kotlin
- Java

### Frameworks
- Spring Boot
- Spring Webflux
- Spring Security
- VueJS

### Databases
- MongoDB
- Redis

### Message Queues/Streams
- Apache Kafka

### Tools
- Auth0
- CI/CD: Github Actions
- Docker
- Kubernetes
- Hosting: Google Cloud Platform

---
## Services
---

### Plugin Store
---

Currently for the plugin store I have 3 microservices:
  - Plugin Service
  - Profile Service
  - Version Service

They all can be found [here](https://github.com/JTM-Network/minecraft-service). The Plugin Store can be found [here](https://www.jtm-network.com/products/store). The aim of the plugin store is to protect the use of these plugins by monitoring the accounts that are using the plugin, and if they are premium, protecting the plugins from being used when shared. Due to the nature of the plugins being virtual goods. I plan to offer protection against malicious chargebacks down the road, by being able to remove access to a resource if that does occur. Understandably you can't protect the source code completely once they receive access to the jar file, however we can make their job harder by using obsfucation.

### Payment
---

The payment service can be found [here](https://github.com/JTM-Network/payment-service). It is currently integrated with stripe which offers one time payments & subscriptions, using debit/credit cards securely. It does not transfer or store user info & card data in order to be PCI Compliant. I plan to add Paypal support in the near future.

