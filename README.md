⚠️ Note: The actual source code is not available due to confidentiality agreements with my previous employer. This project overview is provided to demonstrate my experience and contribution.

# 📊 Springboot-Bulkload-Utility – Spring Boot + Apache POI

A powerful Spring Boot-based utility that enables **bulk upload and download of entity data** using REST APIs with Excel integration. Designed to support static and dynamic fields, this project is ideal for scalable, microservice-driven systems.

🔗 **Live Repo**: [Springboot-Bulkload-Utility](https://github.com/rahulkaparaveni/Springboot-Bulkload-Utility/)

---

## 🚀 Features

- 📥 **Excel Upload API**
  - Parses Excel files using **Apache POI**
  - Handles static fields: `id`, `parentId`, `externalSystemRef`, `fromDate`, `throughDate`
  - Supports dynamic fields prefixed with `fields.` (e.g., `fields.name`, `fields.description`)
  - Validates and stores data into MongoDB

- 📤 **Excel Download API**
  - Exports stored data into a structured Excel format
  - Supports filtering based on query params

- 🧱 **Microservice-Friendly Design**
  - Each service can use its own collection, aligning with microservice architecture best practices

- 📘 **Swagger API Docs**
  - Auto-generated, interactive Swagger UI to explore and test endpoints

- 🛡️ **Robust Error Handling & Validation**
  - Pre-upload validations for clean data ingestion
  - Clear error messages on invalid or malformed data

---

## 🛠️ Tech Stack

| Technology     | Description                           |
|----------------|---------------------------------------|
| Java           | Backend development language          |
| Spring Boot    | Microservice framework                |
| MongoDB        | NoSQL database for dynamic schema     |
| Apache POI     | Excel parsing and writing             |
| Swagger/OpenAPI| REST API documentation and testing    |
| Git & GitHub   | Version control and collaboration     |

---

## 📦 API Endpoints

### ✅ Upload Data
POST /api/v1/data/upload Content-Type: multipart/form-data Body: Excel file (.xlsx)


### ✅ Download Data
GET /api/v1/data/download Query Params: Optional filters


---

## 📈 Project Impact

- Automated bulk operations for internal teams
- Eliminated manual entry errors
- Increased adaptability with dynamic field mapping

---

##🧪 **Testing**

Used JUnit and Mockito for unit testing of core service logic.

Performed integration testing for controller and API endpoints.

Ensured consistent and reliable Excel parsing and database interactions.

Added validation tests for dynamic field mapping and error handling.

---


## 📬 Contact

Developed by **Rahul Kaparaveni**  
📫 Feel free to connect via [Upwork](https://www.upwork.com/freelancers/~0130d13782beaa30aa) or leave a GitHub issue for collaboration or questions.


---

## Documentation

Documented the service design and API workflow using Sequence Diagrams 
Created and maintained technical diagrams using [draw.io](https://app.diagrams.net/) to support development and architectural reviews.


---
