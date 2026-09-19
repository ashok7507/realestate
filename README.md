# 1. Project structure   
```bash
                    REAL ESTATE APPLICATION
                             │
              ┌──────────────┴──────────────┐
              │                             │
              ▼                             ▼
       ANGULAR FRONTEND              SPRING BOOT BACKEND
       localhost:4200                localhost:8080
              │                             │
              │       HTTP / REST API       │
              └─────────────┬───────────────┘
                            │
                            ▼
                    SPRING DATA JPA
                            │
                         Hibernate
                            │
                            ▼
                         MariaDB
                       localhost:3306
```
# 2. Overall Folder Structure  

```bash
real-estate-project/
│
├── frontend/
│   └── new-project/
│
├── backend/
│   └── real-estate-api/
│
└── database/
    ├── schema/
    ├── data/
    └── scripts/
```
# 3. FRONTEND — Angular  
```bash
new-project/
│
├── src/
│   │
│   ├── app/
│   │   │
│   │   ├── core/
│   │   │   ├── guards/
│   │   │   │   ├── auth.guard.ts
│   │   │   │   └── admin.guard.ts
│   │   │   │
│   │   │   ├── interceptors/
│   │   │   │   └── auth.interceptor.ts
│   │   │   │
│   │   │   └── services/
│   │   │       ├── api.service.ts
│   │   │       ├── auth.service.ts
│   │   │       ├── property.service.ts
│   │   │       ├── user.service.ts
│   │   │       ├── favorite.service.ts
│   │   │       └── inquiry.service.ts
│   │   │
│   │   ├── shared/
│   │   │   │
│   │   │   ├── components/
│   │   │   │   ├── navbar/
│   │   │   │   ├── footer/
│   │   │   │   ├── property-card/
│   │   │   │   ├── search-filter/
│   │   │   │   ├── loader/
│   │   │   │   └── pagination/
│   │   │   │
│   │   │   ├── models/
│   │   │   │   ├── property.model.ts
│   │   │   │   ├── user.model.ts
│   │   │   │   ├── inquiry.model.ts
│   │   │   │   └── api-response.model.ts
│   │   │   │
│   │   │   └── pipes/
│   │   │       └── currency-inr.pipe.ts
│   │   │
│   │   ├── pages/
│   │   │   │
│   │   │   ├── home/
│   │   │   │   ├── home.ts
│   │   │   │   ├── home.html
│   │   │   │   └── home.css
│   │   │   │
│   │   │   ├── properties/
│   │   │   │   ├── properties.ts
│   │   │   │   ├── properties.html
│   │   │   │   └── properties.css
│   │   │   │
│   │   │   ├── property-details/
│   │   │   │   ├── property-details.ts
│   │   │   │   ├── property-details.html
│   │   │   │   └── property-details.css
│   │   │   │
│   │   │   ├── add-property/
│   │   │   │   ├── add-property.ts
│   │   │   │   ├── add-property.html
│   │   │   │   └── add-property.css
│   │   │   │
│   │   │   ├── edit-property/
│   │   │   │
│   │   │   ├── login/
│   │   │   │
│   │   │   ├── register/
│   │   │   │
│   │   │   ├── favorites/
│   │   │   │
│   │   │   ├── my-properties/
│   │   │   │
│   │   │   ├── inquiries/
│   │   │   │
│   │   │   └── admin/
│   │   │       ├── dashboard/
│   │   │       ├── users/
│   │   │       └── properties/
│   │   │
│   │   ├── app.ts
│   │   ├── app.html
│   │   ├── app.css
│   │   ├── app.routes.ts
│   │   ├── app.config.ts
│   │   ├── app.config.server.ts
│   │   └── app.routes.server.ts
│   │
│   ├── assets/
│   │   └── images/
│   │
│   ├── index.html
│   └── styles.css
│
├── angular.json
├── package.json
├── tsconfig.json
└── README.md
```
# 4. BACKEND — Spring Boot  
```bash
real-estate-api/
│
├── src/
│   ├── main/
│   │   │
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── realestate/
│   │   │           │
│   │   │           ├── RealEstateApplication.java
│   │   │           │
│   │   │           ├── controller/
│   │   │           │
│   │   │           ├── service/
│   │   │           │
│   │   │           ├── repository/
│   │   │           │
│   │   │           ├── entity/
│   │   │           │
│   │   │           ├── dto/
│   │   │           │
│   │   │           ├── mapper/
│   │   │           │
│   │   │           ├── exception/
│   │   │           │
│   │   │           ├── security/
│   │   │           │
│   │   │           └── config/
│   │   │
│   │   └── resources/
│   │       ├── application.properties
│   │       └── application-dev.properties
│   │
│   └── test/
│
├── pom.xml
└── README.md
```

