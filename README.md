# Grocery Store Database Design

## **Overview**
This database project is a relational database designed to manage and streamline operations for a small grocery store chain with five locations across the United States. This project implements a structured and normalized schema to centralize data for critical business processes such as inventory management, sales tracking, payroll, vendor coordination, and customer interactions.

---

## **Features**
### **Core Functionalities**
- Track inventory levels and automate updates with vendor deliveries and sales.
- Manage employee data, including payroll, schedules, and time tracking.
- Log transactions, including sales and returns, with real-time updates to inventory.
- Support customer loyalty programs and collect customer reviews.
- Enable vendor coordination and delivery tracking.

### **Scalable Design**
- Normalized schema in Third Normal Form (3NF) to reduce redundancy and support future expansion.
- Modular structure for adding new stores, products, or employees.

### **Integrated Tools**
- **ETL Processes**: Real-time integration with the POS system, Employee App, and Website.
- **SQL Views and Stored Procedures**: Predefined queries for advanced reporting and analysis.
- **Metabase Dashboards**: Interactive visualizations for key performance indicators (KPIs) such as sales trends, inventory turnover, and employee performance.
- **Python Integration**: For advanced data manipulation and visualization using libraries like Pandas and SQLAlchemy.

---

## **Technologies Used**
- **Database**: PostgreSQL
- **Tools**: pgAdmin, Metabase
- **Programming Languages**: SQL, Python

---

## **Schema Overview**
The database consists of 20 tables, including:
- **Core Tables**: `Store`, `Employee`, `Department`, `Products`, `Transactions`.
- **Specialized Tables**: `Payroll`, `Sales`, `Price_History`, `Inventory`, `Customer_Reviews`, `Product_Waste`.

### **Relationships**
- **One-to-Many**: Stores → Employees, Vendors → Products.
- **Many-to-Many**: Products ↔ Transactions (via Sales).
---

## **License**
This project is licensed under the [MIT License](LICENSE).
