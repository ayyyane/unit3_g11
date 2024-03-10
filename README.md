# unit3 project

## CriteriaA
<img width="469" alt="Screenshot 2024-03-08 at 16 34 44" src="https://github.com/ayyyane/unit3_g11/assets/142702159/0a9dc49a-df2a-49fa-8e7a-c2089be47450">

## Problem definition
A lady runs the company which produces water bottles alone. She faces the problems of tracing customers' orders, materials, and money. The problems led to mistakes in calculating sales　and sending products to a different customer which made the negative repetition to her company. She has been keeping a paper record with all this information since she does not know much about the computer. She also wants to hire a new employee to support managing customer requests and purchasing materials, however, she does not want to share her paper record since it contains confidential information (money), yet the staff needs to see orders and materials. She is in a pickle.



## Proposed Solution
I will provide an application to trace customers order, materials and money with the tools below.

Justification of tools:
 Python, Kivy, and SQLite offer a comprehensive solution for the client's business needs. Python, as a versatile and easy-to-learn programming language, provides a robust framework for developing custom software tailored to the client's specific requirements. Its simplicity and readability make it ideal for individuals with limited computer knowledge, enabling the client to understand and potentially even modify the software in the future. Moreover, Python's extensive ecosystem boasts numerous libraries and frameworks that can streamline development and enhance functionality, ensuring a tailored solution to the client's challenges.

Kivy, a Python framework for developing multi-touch applications, is particularly advantageous for the client's situation. Its cross-platform nature allows for the creation of user-friendly interfaces that can run seamlessly on various devices, including desktops, tablets, and smartphones. By leveraging Kivy, the client can develop an intuitive application that simplifies the management of customer orders, materials, and finances. The graphical user interface (GUI) provided by Kivy enables the client and her potential employees to interact with the software effortlessly, facilitating efficient data entry, retrieval, and analysis.

SQLite serves as an efficient and lightweight database management system, perfectly suited for the client's needs. Its self-contained, serverless architecture eliminates the need for complex setup and maintenance, making it an ideal choice for small-scale applications. With SQLite, the client can securely store and manage sensitive data, such as customer orders and financial records, without the need for extensive technical expertise. Furthermore, SQLite seamlessly integrates with Python, allowing for seamless interaction between the application's front end developed using Kivy and the backend database. This integration ensures data consistency, reliability, and confidentiality, addressing the client's concerns regarding the security of her confidential information while enabling her staff to access necessary data for managing customer requests and material procurement.

## Success Criteria

1. The application allows the client to trace the money clearly using orders and expenses. Trace includes creating, editing, and deleting orders or expenses. [Issue Trackled: "She faces the problems of tracing customers orders, materials and money."]
2. The application allows the client to track the amount of raw materials needed for the water bottle. Tracing shows the amount of metal, plastic,  [Issue Trackled: "She faces the problems of tracing customers orders, materials and money."]
3. The application allows the client to produce water bottles by pushing a few buttons and entering the information. (Issue Trackled: "She has been keeping a paper record with all this information since she does not know much about the computer.")
4. The application has a login system and a signup system for hiring the new employee.[Issue Trackled: ”She also wants to hire a new employee in order to support managing customer requests and purchasing materials]
5. The application has two menus separated by the positions, managers, or staff which only allows for managers to see the finance information. [Issue Trackled: she does not want to share her paper record since it contains confidential information (money), yet the staff needs to see orders and materials. She is in a pickle.]

## Criteria B Design

## System Diagram
<img width="1020" alt="systemdiagram" src="https://github.com/ayyyane/unit3_g11/assets/142702159/ed208c75-f556-4ab4-b2f9-056cc50359a9">

**fig.** shows the system diagram

The system diagram provides a visual representation of the system, its parts, and how they relate to one another. This displays the input (keyboard) to the output (various systems used in this project, including versions of the programming language (Python and KivyMD), the computer version and detail (Processor, version, memory, etc.), the module and database, and the output screen (application interface on the computer screen).

## Wireframe Diagram
![Wireframediagram](https://github.com/ayyyane/unit3_g11/assets/142702159/75d77dce-bfc3-4d9a-adcd-a108999eef9c)

**fig** shows the Wireframe diagram

This wireframe diagram's objective is to visually represent the user interface design that outlines the application's structure and layout. The wireframe also shows how various screens will be accessed via various buttons. The user can see which screen will open when they touch and release the button according to the arrows that extend from the button to the screen.

## Flow Diagram
## ER Diagram
<img width="1095" alt="ER diagram" src="https://github.com/ayyyane/unit3_g11/assets/142702159/401c2215-c2f6-4902-ab79-72089063b101">

**fig** shows the ER diagram

This is the ER diagram for the database illustrating the relationship between the items table and users table from the database, called "project3.db". In the users table, there are 4 different columns including id, name, hash, and post each column will have the specific data type after the column name. The second table orders has 8 columns which are id, date, number, phone, products, price, and name. The last table inventory has two columns, amount and name.

## UML Diagram
<img width="1051" alt="UMLdiagram" src="https://github.com/ayyyane/unit3_g11/assets/142702159/41c4d723-2472-4edb-bc84-574552cbc394">

**fig**

This UML diagram for the OOP classes illustrates the classes and methods utilized during the development of the application. It showcases two primary parent classes, namely MDApp and MDScreen. All the classes inherit the methods and attributes of these parent classes, which is demonstrated by the arrows displayed on the diagram.

## Test Plan

## Record of task
| Task No | Planned Action                                                                                                              | Planned outcome                                                                                                                               | Time estimeat | Target complete date | Criterioin |
|---------|-----------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------|------------|
| 1       | Meet with the client                                                                                                        | talk with the client to discuss the problems she is facing and brainstorm solutions to create a plan to help the client resolve the problems. | 15 min        | Feb 20               | A          |
| 2       | Brainstorm and write the problems definition                                                                                | A clear problem definition of what the client is facing.                                                                                      | 20 min        | Feb 20               | A          |
| 3       | Write proposed solution                                                                                                     | A clear justification that suits the client and developer.                                                                                    | 15 min        | Feb 21               | A          |
| 4       | Brainstorm and write down success criteria                                                                                  | A clear success criteria that suits the client and resolves the problem.                                                                      | 20 min        | Feb 21               | A          |
| 5       | Brainstorm and write down a design statement for the client                                                                 | A clear design statement that suits the need of the client.                                                                                   | 15 min        | Feb 21               | A          |
| 6       | Write flow diagrams                                                                                                         | flowcharts and a brief explanation for each section of the solution to obtain a clearer understanding of the code's proccess                  | 1 hour        | Feb 21               |            |
| 7       | Create system diagram                                                                                                       | To have a clear idea of the hardware and software requirements for the proposed solution                                                      | 1 hour        | Feb 22               | A          |
| 8       | Draw a wire frame and write an explanation                                                                                  | Have a clear wire frame that accurately represents and describes the application and have a brief explanation.                                | 1 hour        | Feb 22               | B          |
| 9       | Client meeting                                                                                                              | Present success criteria to client to get the approval.                                                                                       | 15min         | Feb 23               | A          |
| 10      | Create basic screens(Login page, Signup page, ManagerMenu, StaffMenu, FinancePage, CustomerPage, OrderPage, InventoryPage ) | User can go to other page when user push the button.                                                                                          | 45min         | Feb 23               | C          |
| 11      | Add home button in the screens including FinancePage, CustomerPage, OrderPage and InventoryPage.                            | The screen changes to either ManagerMenu or StaffMenu depending on the position of the user when user push the home button.                   | 30min         | Feb 23               | C          |
| 12      | Create login&Signup system                                                                                                  | A working login and signup screen with Python and KivyMD with a GUI                                                                           | 3 hours       | Feb24                | C          |
| 13      | Create show password function                                                                                               | Make user to see the password                                                                                                                 | 15min         | Feb24                | C          |
| 14      | Create order system                                                                                                         | The data including date, number, phone, products, price and name are saved to the database when user input them.                              | 1 hour        | Feb 26               | C          |
| 15      | Add date picker                                                                                                             | User can chose the date the customer order easily.                                                                                            | 1 hour        | Feb 26               | C          |
| 16      | Add dropdown box                                                                                                            | User can choose the material of the product without the mistakes including spell mistakes.                                                    | 1.5 hour      | Feb 28               | C          |
| 17      | Create on_pre function                                                                                                      | User can see the amount of material saved in inventory table when the screen is changed to InventoryPage.                                     | 1 hour        | Feb 29               | C          |
| 18      | Create produce button                                                                                                       | The amount of material is reduced when user push the produce button.                                                                          | 2 hour        | Feb 29               | C          |
| 19      | Add dropdown box to produce button                                                                                          | User can choose the material of products without any spell mistakes.                                                                          | 1.5 hour      | March 1              | C          |
| 20      | Create add system                                                                                                           | User can add the amount of materials and the new data is saved to the table called inventory.                                                 | 1 hour        | March 1              | C          |
| 21      | Add logout button in ManagerMenu and StaffMeni                                                                              | User can go back to loginscreen when user push the button logout.                                                                             | 30 min        | March 2              | C          |
| 22      | Add hash in user table                                                                                                      | The hash is saved instead of saving password into the table to keep the users' information safety.                                            | 1 hour        | March 2              | C          |
| 23      | Finish test plans                                                                                                           | Contains the procedures for testing the application as well as the expected results of each test.                                             | 2 hours       | March 5              | B          |
| 24      | Write CriteriaC                                                                                                             | Write the code descriptions as well as the specifics of the techniques implemented.                                                           | 2 hours       | March 7              | C          |
| 25      | Film final video                                                                                                            | Video demonstration of all success criterias operating and functioning within the built application                                           | 1 hours       | March 8              |            |
