# Fusion Security Lab

## What I did today (Day 1)
- Opened Security Console successfully
- Inspected my user roles:
  - Application Implementation Consultant
  - IT Security Manager
  - Employee
- Explored seeded role: Employee
  - Interesting Duty: Employee Self-Service Duty
  - Notable Function Security Policy: View Person Profile → allows employee to view their own profile
  - Notable Data Security Policy: Access to Person Records → restricts access so user sees only their own data

## Notes to self
- Role Hierarchy shows which duties a role inherits
- Function Security Policies control **what tasks/actions** a user can perform in UI
- Data Security Policies control **what data** a user can access (e.g., only their own department)
- Missing roles: none for now (I already have IT Security Manager + AIC)

## Next up
- Create a small custom role and assign it to a test user

## Screen shots
- <img width="1919" height="949" alt="Screenshot 2025-08-22 141310" src="https://github.com/user-attachments/assets/07642829-55b2-4eb9-9262-0a6d93ba7336" />
- <img width="1911" height="947" alt="Screenshot 2025-08-22 141346" src="https://github.com/user-attachments/assets/eebbf2f7-3143-4038-ab28-3bbbab95a2bb" />
- <img width="1919" height="950" alt="Screenshot 2025-08-22 142104" src="https://github.com/user-attachments/assets/ec120118-aad2-44d3-830d-ee4068dddace" />
- <img width="1919" height="949" alt="Screenshot 2025-08-22 142134" src="https://github.com/user-attachments/assets/5907d462-a82e-4bc9-82ef-1fabb9158203" />


## Day 1 (Part 2) – Custom Role and Test User

- Created custom role: XX_CUSTOM_EMPLOYEE_ROLE
  - Added Function Security: View Person Profile
  - Added Data Security: View own Person record
 
- Created new test user: TEST_EMPLOYEE1
 
- Assigned custom role to the test user

## Screen shots
- <img width="1916" height="937" alt="Screenshot 2025-08-22 151823" src="https://github.com/user-attachments/assets/02a4cdf7-1235-4387-a9e9-622d8ce40a71" />
- <img width="1826" height="989" alt="Screenshot 2025-08-22 161330" src="https://github.com/user-attachments/assets/85196f08-e5f8-423c-8471-e79f21a5ee6e" />
- <img width="1650" height="828" alt="Screenshot 2025-08-22 155658" src="https://github.com/user-attachments/assets/28e11640-4f22-4667-a864-6c09edb3482e" />




