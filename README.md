# e-commerce
Scalable E-Commerce Platform
┌───────────────────────────────────────────────────────────────────────┐
│                            E-Commerce Platform                       │
├─────────────────┬─────────────────┬─────────────────┬────────────────┤
│  API Gateway    │  Service        │  Service        │  Service       │
│  (Spring Cloud  │  Discovery      │  Registry       │  Config        │
│  Gateway)       │  (Eureka)       │  (Eureka)       │  Server        │
└─────────────────┴─────────────────┴─────────────────┴────────────────┘
          ▲                ▲                ▲                ▲
          │                │                │                │
┌─────────┴────┐   ┌───────┴──────┐   ┌─────┴──────┐   ┌─────┴──────┐
│ Product      │   │ User         │   │ Shopping   │   │ Order      │
│ Service      │   │ Service      │   │ Cart       │   │ Service    │
│ (Spring Boot)│   │ (Spring Boot)│   │ Service    │   │ (Spring    │
└──────────────┘   └──────────────┘   │ (Spring    │   │ Boot)      │
                                      │ Boot)      │   └────────────┘
┌──────────────┐   ┌──────────────┐   └────────────┘   ┌────────────┐
│ Payment      │   │ Inventory    │   ┌────────────┐   │ Email      │
│ Service      │   │ Service      │   │ Review      │   │ Service    │
│ (Spring Boot)│   │ (Spring Boot)│   │ Service    │   │ (Spring    │
└──────────────┘   └──────────────┘   │ (Spring    │   │ Boot)      │
                                      │ Boot)      │   └────────────┘
                                      └────────────┘
