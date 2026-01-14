<br>

```mermaid

sequenceDiagram
    participant User as Employee
    participant Assistant as HR Portal AI Assistant
    participant HRMS as HR Management System
    
    User->>Assistant: "What is my leave balance?"
    Assistant->>HRMS: Request for leave balance of employee
    HRMS-->>Assistant: Return leave balance
    Assistant-->>User: "You have 5 annual leaves remaining."
    
    User->>Assistant: "Show my latest payslip."
    Assistant->>HRMS: Request for latest payslip of employee
    HRMS-->>Assistant: Return latest payslip details
    Assistant-->>User: "Here is your latest payslip for August 2024."
    
    User->>Assistant: "How can I apply for sick leave?"
    Assistant-->>User: "You can apply for sick leave through this form. [Leave Application Form]"

    User->>Assistant: "Who is my HR representative?"
    Assistant->>HRMS: Request HR representative for employee's department
    HRMS-->>Assistant: Return HR representative details
    Assistant-->>User: "Your HR representative is Jane Doe."
    
    User->>Assistant: "Can I update my bank account information?"
    Assistant-->>User: "You can update your bank details through the payroll section. [Update Bank Info]"
    
    User->>Assistant: "Schedule my annual leave starting next Monday."
    Assistant->>HRMS: Request leave scheduling for employee
    HRMS-->>Assistant: Leave request submitted successfully
    Assistant-->>User: "Your leave from next Monday has been successfully scheduled."

