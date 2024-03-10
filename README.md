# unit3 project

## CriteriaA
<img width="469" alt="Screenshot 2024-03-08 at 16 34 44" src="https://github.com/ayyyane/unit3_g11/assets/142702159/0a9dc49a-df2a-49fa-8e7a-c2089be47450">

**fig1** shows the photo of waterbottle

### Problem definition
A lady runs the company which produces water bottles alone. She faces the problems of tracing customers' orders, materials, and money. The problems led to mistakes in calculating sales　and sending products to a different customer which made the negative repetition to her company. She has been keeping a paper record with all this information since she does not know much about the computer. She also wants to hire a new employee to support managing customer requests and purchasing materials, however, she does not want to share her paper record since it contains confidential information (money), yet the staff needs to see orders and materials. She is in a pickle.



### Proposed Solution
I will provide an application to trace customers' orders, materials, and money with the tools below.

Justification of tools:
 Python, Kivy, and SQLite offer a comprehensive solution for the client's business needs. Python, as a versatile and easy-to-learn programming language, provides a robust framework for developing custom software tailored to the client's specific requirements. Its simplicity and readability make it ideal for individuals with limited computer knowledge, enabling the client to understand and potentially even modify the software in the future. Moreover, Python's extensive ecosystem boasts numerous libraries and frameworks that can streamline development and enhance functionality, ensuring a tailored solution to the client's challenges.

Kivy, a Python framework for developing multi-touch applications, is particularly advantageous for the client's situation. Its cross-platform nature allows for the creation of user-friendly interfaces that can run seamlessly on various devices, including desktops, tablets, and smartphones. By leveraging Kivy, the client can develop an intuitive application that simplifies the management of customer orders, materials, and finances. The graphical user interface (GUI) provided by Kivy enables the client and her potential employees to interact with the software effortlessly, facilitating efficient data entry, retrieval, and analysis.

SQLite serves as an efficient and lightweight database management system, perfectly suited for the client's needs. Its self-contained, serverless architecture eliminates the need for complex setup and maintenance, making it an ideal choice for small-scale applications. With SQLite, the client can securely store and manage sensitive data, such as customer orders and financial records, without the need for extensive technical expertise. Furthermore, SQLite seamlessly integrates with Python, allowing for seamless interaction between the application's front end developed using Kivy and the backend database. This integration ensures data consistency, reliability, and confidentiality, addressing the client's concerns regarding the security of her confidential information while enabling her staff to access necessary data for managing customer requests and material procurement.

### Success Criteria

1. The application allows the client to trace the money clearly using orders and expenses. Trace includes creating, editing, and deleting orders or expenses. [Issue Trackled: "She faces the problems of tracing customers orders, materials and money."]
2. The application allows the client to track the amount of raw materials needed for the water bottle. Tracing shows the amount of metal, plastic,  [Issue Trackled: "She faces the problems of tracing customers orders, materials and money."]
3. The application allows the client to produce water bottles by pushing a few buttons and entering the information. (Issue Trackled: "She has been keeping a paper record with all this information since she does not know much about the computer.")
4. The application has a login system and a signup system for hiring the new employee.[Issue Trackled: ”She also wants to hire a new employee in order to support managing customer requests and purchasing materials]
5. The application has two menus separated by the positions, managers, or staff which only allows for managers to see the finance information. [Issue Trackled: she does not want to share her paper record since it contains confidential information (money), yet the staff needs to see orders and materials. She is in a pickle.]

## Criteria B Design

### System Diagram
<img width="1020" alt="systemdiagram" src="https://github.com/ayyyane/unit3_g11/assets/142702159/ed208c75-f556-4ab4-b2f9-056cc50359a9">

**fig2.** shows the system diagram

The system diagram provides a visual representation of the system, its parts, and how they relate to one another. This displays the input (keyboard) to the output (various systems used in this project, including versions of the programming language (Python and KivyMD), the computer version and detail (Processor, version, memory, etc.), the module and database, and the output screen (application interface on the computer screen).

### Wireframe Diagram
![Wireframediagram](https://github.com/ayyyane/unit3_g11/assets/142702159/75d77dce-bfc3-4d9a-adcd-a108999eef9c)

**fig3** shows the Wireframe diagram

This wireframe diagram's objective is to visually represent the user interface design that outlines the application's structure and layout. The wireframe also shows how various screens will be accessed via various buttons. The user can see which screen will open when they touch and release the button according to the arrows that extend from the button to the screen.

### Flow Diagram

### signup system
<img width="579" alt="flowchart1" src="https://github.com/ayyyane/unit3_g11/assets/142702159/e9d112b5-4e30-4c88-838b-a2679b8709b4">

**fig4** The flow diagram of signup system

This is the flow diagram for the code to sign up. This code collects data including username, password, cpass(confirm password), and post(position). This function firstly check if the password and cpass matches and nextly if the post is either 'manager' or 'staff'. After that, make sure that there's no user with the same name and add this information in the database.

### login system
<img width="437" alt="Screenshot 2024-03-11 at 1 49 30" src="https://github.com/ayyyane/unit3_g11/assets/142702159/ed33c16a-1073-430c-bca9-69bcc325ecb8">

**fig5** The flow diagram of login system

This is the flow diagram for the code to login. This code collects data including username, and password. This function first checks the hash where the username is saved and checks the hash is the same as the produced hash with the input password.

## calculator in FinancePage
<img width="401" alt="Screenshot 2024-03-11 at 1 59 38" src="https://github.com/ayyyane/unit3_g11/assets/142702159/4a813bdd-788d-4399-9364-3cfb32af6e60">

**fig6** The flow diagram of the calculator

This is the flow diagram for the code to calculate the proceeds. This code collects data to date. Then search the database where the date matches with input date and calculate the total proceeds in the month.



### ER Diagram
<img width="1095" alt="ER diagram" src="https://github.com/ayyyane/unit3_g11/assets/142702159/401c2215-c2f6-4902-ab79-72089063b101">

**fig7** shows the ER diagram

This is the ER diagram for the database illustrating the relationship between the items table and users table from the database, called "project3.db". In the users table, there are 4 different columns including id, name, hash, and post each column will have the specific data type after the column name. The second table orders has 8 columns which are id, date, number, phone, products, price, and name. The last table inventory has two columns, amount and name.

### UML Diagram
<img width="1051" alt="UMLdiagram" src="https://github.com/ayyyane/unit3_g11/assets/142702159/41c4d723-2472-4edb-bc84-574552cbc394">

**fig8** shows the UML diagram

This UML diagram for the OOP classes illustrates the classes and methods utilized during the development of the application. It showcases two primary parent classes, namely MDApp and MDScreen. All the classes inherit the methods and attributes of these parent classes, which is demonstrated by the arrows displayed on the diagram.

### Test Plan
| Description               | Test type                    | input                                                                                                                                                                                               | Explected output                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|---------------------------|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Signup system             | unit test                    | 1. Run the project. 2. Click the "SignUp" button. 3. Input the information required on the screen. 4. Click "see password" button. 5. Click "submit" button.                                        | After clicking the "Submit" button, the Screen shifts to either "ManagerPage" or "StaffPage" depending on the users' input "position". If the user input "manager", shift to "ManagerPage" and if the user inputs "staff", shift to "StaffPage". Also, the textbox is changed to red if the user does occur the error including the different text type input and not matching the password and the confirm password.  If the "see password" button is clicked, user can see the password. |
| Login system              | unit test                    | 1. Run the project. 2. Enter the information in the text field on the screen. 3. Click the "login" button.                                                                                          | After entering all the appropriate information and if the user can log in successfully, the screen shifts to either "ManagerPage" or "StaffPage" the same as the signup system. If the user presses the "Login" button the user does not exist or the password doesn't match, the error message will appear letting the user know that the login failed.                                                                                                                                   |
| Move to each screen       | integration test             | 1. Run the project. 2. Login 3. Click the each button which has a text of the name of screen. 4. Click the home button on the shifted screen.                                                       | After clicking the button on the Menu, the scrren is shifted to the screen which name is the same as the text on the button. If home button on the shifted screen is clicked, the screen is changed to the Menu.                                                                                                                                                                                                                                                                           |
| Finance system            | unit test                    | 1. Run the project. 2. Login 3. Click the "Finance" button. 3. Add "2024-02" on the text field. 4. Add "2024-03" on the text field. 5. Click the "show the finance information" button.             | After entering "2024-02", the error message is shown on the screen. After entering "2024-03", the proceeds is shown on the screen.                                                                                                                                                                                                                                                                                                                                                         |
| Order and Customer system | unit test & integration test | 1. Run the project. 2. Login 3. Click the "Order" button. 4. Add information required on the screen. 5. Push the "save" button.                                                                     | If the added information is different with the requirement, the error message is shown. After clicking the "save" button with accurate information, the screen is changed to "CustomerPage" and the information is added to the table.                                                                                                                                                                                                                                                     |
| Inventory system          | unit test                    | 1. Run the project. 2. Login 3. Click the "Inventory" button. 4. Click produce button and chose optioin on the drop down box. 5. Add the amount number in the text field. 6. Click the save button. | The amount of material is decreased when the button with the text of the material is clicked. After information is added in the textfield and the "save" button is clicked, the amount is increased.                                                                                                                                                                                                                                                                                       |
| Logout button             | integration test             | 1. Run the project. 2. Login 3. Click "Logout"button.                                                                                                                                               | After the button is pressed, the screen is changed to "LoginPage" and the password is invisible.                                                                                                                                                                                                                                                                                                                                                                                           |

### Record of task
| Task No | Planned Action                                                                                                              | Planned outcome                                                                                                                               | Time estimate | Target complete date | Criterion |
|---------|-----------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------|------------|
| 1       | Meet with the client                                                                                                        | Talk with the client to discuss the problems she is facing and brainstorm solutions to create a plan to help the client resolve the problems. | 15 min        | Feb 20               | A          |
| 2       | Brainstorm and write the problem definition                                                                                | A clear problem definition of what the client is facing.                                                                                      | 20 min        | Feb 20               | A          |
| 3       | Write proposed solution                                                                                                     | A clear justification that suits the client and developer.                                                                                    | 15 min        | Feb 21               | A          |
| 4       | Brainstorm and write down success criteria                                                                                  | A clear success criteria that suits the client and resolves the problem.                                                                      | 20 min        | Feb 21               | A          |
| 5       | Brainstorm and write down a design statement for the client                                                                 | A clear design statement that suits the needs of the client.                                                                                   | 15 min        | Feb 21               | A          |
| 6       | Write flow diagrams                                                                                                         | flowcharts and a brief explanation for each section of the solution to obtain a clearer understanding of the code's process                  | 1 hour        | Feb 21               |            |
| 7       | Create system diagram                                                                                                       | To have a clear idea of the hardware and software requirements for the proposed solution                                                      | 1 hour        | Feb 22               | A          |
| 8       | Draw a wire frame and write an explanation                                                                                  | Have a clear wire frame that accurately represents and describes the application and have a brief explanation.                                | 1 hour        | Feb 22               | B          |
| 9       | Client meeting                                                                                                              | Present success criteria to the client to get approval.                                                                                       | 15min         | Feb 23               | A          |
| 10      | Create basic screens(Login page, Signup page, ManagerMenu, StaffMenu, FinancePage, CustomerPage, OrderPage, InventoryPage ) | User can go to other pages when the user pushes the button.                                                                                          | 45min         | Feb 23               | C          |
| 11      | Add a home button in the screens including FinancePage, CustomerPage, OrderPage, and InventoryPage.                            | The screen changes to either ManagerMenu or StaffMenu depending on the position of the user when the user pushes the home button.                   | 30min         | Feb 23               | C          |
| 12      | Create login&Signup system                                                                                                  | A working login and signup screen with Python and KivyMD with a GUI                                                                           | 3 hours       | Feb24                | C          |
| 13      | Create show password function                                                                                               | Make user to see the password                                                                                                                 | 15min         | Feb24                | C          |
| 14      | Create order system                                                                                                         | The data including date, number, phone, products, price, and name are saved to the database when the user inputs them.                              | 1 hour        | Feb 26               | C          |
| 15      | Add date picker                                                                                                             | User can chose the date the customer order easily.                                                                                            | 1 hour        | Feb 26               | C          |
| 16      | Add dropdown box                                                                                                            | The User can choose the material of the product without the mistakes including spelling mistakes.                                                    | 1.5 hour      | Feb 28               | C          |
| 17      | Create on_pre function                                                                                                      | The User can see the amount of material saved in the inventory table when the screen is changed to InventoryPage.                                     | 1 hour        | Feb 29               | C          |
| 18      | Create produce button                                                                                                       | The amount of material is reduced when the user pushes the produce button.                                                                          | 2 hour        | Feb 29               | C          |
| 19      | Add a dropdown box to produce button                                                                                          | User can choose the material of products without any spelling mistakes.                                                                          | 1.5 hour      | March 1              | C          |
| 20      | Create add system                                                                                                           | User can add the amount of materials and the new data is saved to the table called inventory.                                                 | 1 hour        | March 1              | C          |
| 21      | Add logout button in ManagerMenu and StaffMeni                                                                              | User can go back to the login screen when the user pushes the button logout.                                                                             | 30 min        | March 2              | C          |
| 22      | Add hash in user table                                                                                                      | The hash is saved instead of saving the password into the table to keep the users' information safe.                                            | 1 hour        | March 2              | C          |
| 23      | Finish test plans                                                                                                           | Contains the procedures for testing the application as well as the expected results of each test.                                             | 2 hours       | March 5              | B          |
| 24      | Write CriteriaC                                                                                                             | Write the code descriptions as well as the specifics of the techniques implemented.                                                           | 2 hours       | March 7              | C          |
| 25      | Film final video                                                                                                            | Video demonstration of all success criteria operating and functioning within the built application                                           | 1 hour       | March 8              |            |


## criteria C development

## Technic used
1. OOP paradigm
2. KivyMD Library
3. Relational databases
4. SQLite, ORM
5. functions
6. if statements

 ## Python file: "project3.py"

 ### Setting up the file

 ```.py
import sqlite3

from kivy.lang import Builder
from kivymd.app import MDApp
from kivymd.uix.datatables import MDDataTable
from kivymd.uix.menu import MDDropdownMenu
from kivymd.uix.pickers import MDDatePicker
from kivymd.uix.screen import MDScreen

```
The code imports several libraries that will be used to build the application. The sqlite3 library is used to connect to and manipulate an SQLite database, which will be used to store the data. The kivymd library is used to build the graphical user interface (GUI) of the application, which will be user-friendly and easy to navigate.

### DatabaseBridge

The class called DatabaseBridge initializes a connection to a SQLite database with the given name. It abstracts away the details of connecting to a database allowing the developer to interact with the database through a simplified interface. 

```.py
 def __init__(self, name:str, ):
        self.db_name = name
        self.connect = sqlite3.connect(self.db_name) # connecting the database called self.db_name and define to use sqlite3
        self.cursor = self.connect.cursor()

```
This code defines an __init__ method within a class, which initializes an object with a specified database name. The __init__ method takes a string parameter name, representing the name of the database. Inside the method, it assigns the provided name to the db_name attribute of the object. It then establishes a connection to the SQLite database specified by db_name using the sqlite3.connect() function, and assigns the connection object to the connect attribute. Additionally, it creates a cursor object for executing SQL commands on the database and assigns it to the cursor attribute. Overall, this code snippet sets up a connection to a SQLite database within an object, enabling subsequent interactions with the database through the created cursor.

### Create/check hash

```.py
def get_hash(text:str):
    return hash_function.hash(text)

def check_hash(input_hash, text): # check if the hash is same
    return hash_function.verify(text, input_hash)
```
 The first function get_hash() takes a string text as input and returns the hash value of that text using a hash function hash_function.hash(). The second function check_hash() is designed to verify if a given hash value input_hash corresponds to the original text text. It takes two parameters: the hash value to check and the original text. It then utilizes a hash verification function hash_function.verify() to compare the provided hash value with the hash generated from the original text. The function returns True if the hashes match, indicating that the original text hasn't been tampered with, and False otherwise. These functions are useful for securely storing and verifying sensitive information such as passwords or digital signatures within an application.

### Signup system

```.py
    def try_signup(self):
        password = self.ids.password.text
        cpass = self.ids.cpass.text

        if password != cpass:
            self.ids.cpass.error = True
        # the passwords match
        # check the password policy, length etc
        post = self.ids.post.text  # get the email from GUI
        if post != 'manger' or post != 'staff':
            self.ids.post.error = True

        # assume that you checked the username as well
        username = self.ids.username.text

        # check if the user have already existed
        uname = f"SELECT name FROM users WHERE name = '{username}'"
        results = project3.db.search(query=uname, multiple=True)
        hash = get_hash(password)

        if results == []:
            new_user = f"""INSERT into users(post, hash, name) 
            values('{post}', '{hash}', '{username}')
                            """

            if post == 'manager':
                self.parent.current = 'ManagerMenu'
                project3.db.insert(insert_query=new_user)
                self.ids.password.text= ""


            elif post == 'staff':
                self.parent.current = "StaffMenu"
                project3.db.insert(insert_query=new_user)
                self.ids.password.text = ""

            else:
                self.ids.post.error = True

        else:
            self.ids.username.error = True

```


try_signup is a class in SignupScreen, presumably associated with a graphical user interface (GUI). The method retrieves input data such as password, confirmed password, post, and username from the GUI elements. It performs several checks on the input data: firstly, it compares the password and confirmed password to ensure they match, displaying an error if they don't. Then, it verifies if the post input matches predefined values 'manager' or 'staff', displaying an error if it doesn't. Next, it checks if the provided username already exists in the database. If the username doesn't exist, it creates a new user entry in the database with the provided details (post, hash of the password, username), and redirects the user to either 'ManagerMenu' or 'StaffMenu' based on the role specified. If the username already exists, it displays an error indicating that the user already exists. In this method, a hash is saved instead of saving the password.

### Login system
```.py
position = None
    def check_user(self):
        db_name = "project3.db"
        project3.db = DatabaseBridge(db_name)
        username = self.ids.username.text
        password = self.ids.password.text
        self.ids.username.error = False
        self.ids.password.error = False


        query_hash = f"""Select hash from users where name = '{username}'"""
        results_hash = project3.db.search(query=query_hash, multiple=True)
        print(results_hash[0][0],password)
        query_post =  f"""Select post from users where name = '{username}'"""
        results_post = project3.db.search(query=query_post, multiple=True)
        print(check_hash(results_hash[0][0],password))
        print(results_post)

        if check_hash(results_hash[0][0],password) == True:
            LoginScreen.position = results_post[0][0]
            print(LoginScreen.position)
            print("hello")
            if results_post[0][0] == "manager":
                self.parent.current = "ManagerMenu"
                self.ids.password.text = ""
            else:
                self.parent.current = "StaffMenu"
                self.ids.password.text = ""
        else:
            self.ids.password.error = True

```
The method retrieves the username and password input from the GUI elements and initializes error flags for potential error states. It then queries a database to retrieve the hash of the password corresponding to the provided username. If the hash of the provided password matches the stored hash in the database, it sets the user's position (manager or staff) and navigates to the appropriate menu screen within the GUI. If the password verification fails, it flags an error on the password input field. This code segment serves as part of a user authentication mechanism, verifying user credentials against a stored database of usernames and hashed passwords before granting access to different parts of the application based on the user's role.

### create table
```.py
def create_finance(self):
    query = """Create table if not exists finance(
                          id integer primary key,
                          date str,
                          amount int,
                          purpose str
                          )"""
    project3.db.run_query(query=query)

```
The method is responsible for creating a table named "finance" if it doesn't already exist in the database. The SQL query string defines the structure of the "finance" table, specifying columns such as 'id', 'date', 'amount', and 'purpose'. The method then executes this query using a database interaction object project3.db.run_query(). Overall, this code segment automates the creation of a financial data table in the database, ensuring its existence before performing any subsequent operations involving financial data storage or retrieval within the application.

### show table on the screen
```.py
    def on_pre_enter(self, *args):
        # [name,size]
        column_name = [('id', 40),('date',40),('products',30),('number',40),('price',30),('name', 50), ('phone', 50)]

        self.data_table = MDDataTable(
            size_hint=(.7, .5),
            pos_hint={'center_x': .5, 'top': .7},
            use_pagination=True,
            check=True,
            column_data=column_name
        )
        self.data_table.bind(on_row_press=self.row_pressed)
        self.data_table.bind(on_check_press=self.check_pressed)
        self.add_widget(self.data_table)
        self.update()
```
This code defines a set of column names along with their sizes to be used in a data table. The MDDataTable widget from the KivyMD library is then instantiated with specified properties such as size hint, position hint, pagination usage, and check functionality, and initialized with the column data. Event bindings for row press and check press events are attached to the data table, indicating actions to be performed when a row is pressed or checked. Finally, the data table is added to the GUI, and the update() method is called, possibly to populate the table with initial data. This code segment sets up a data table within the GUI, providing an interface for displaying and interacting with tabular data in the application.

### Save
```.py
def save(self):
        name = self.ids.name.text
        products = self.ids.products.text
        number = self.ids.number.text
        date = self.ids.date.text
        phone = self.ids.phone.text
        price = self.ids.price.text
        save_q = f"""INSERT INTO orders(date, products, number, price, name, phone) 
                    VALUES ('{date}','{products}',{number},{price},'{name}',{phone})"""
        project3.db.run_query(query=save_q)
        self.update()
        self.parent.current = "CustomerPage"
        project3.db.run_query(query=save_q)
```

This method retrieves input data such as customer name, ordered products, quantity, date, contact phone number, and price from the graphical user interface (GUI) elements. It constructs an SQL query string save_q to insert this data into an "orders" table within a database. The method then executes this query using a database interaction object project3.db.run_query(). After updating the GUI to reflect the changes, it navigates the user back to the "CustomerPage". However, there seems to be redundancy in the execution of the SQL query, as it's being executed twice consecutively with the same query string. This code segment essentially facilitates the saving of order details into the database and transitioning the user to another page within the application after the operation is completed.

### Drop down menu
```.py
    def DropDownMenu(self, button):
        print("working DropDownMenu")
        button_menu = [{'text':"Glass",
                        'viewclass':"OneLineListItem",
                        'on_release': lambda x='': self.check_material("glass")},
                       {'text': "Stainless steel",
                        'viewclass': "OneLineListItem",
                        'on_release': lambda x='text': self.check_material("stainless steel")},
                       {'text': "Aluminium",
                        'viewclass': "OneLineListItem",
                        'on_release': lambda x='text': self.check_material("aluminium")},
                       {'text': "Plastic",
                        'viewclass': "OneLineListItem",
                        'on_release': lambda x='text': self.check_material("plastic")}
        ]

        self.menu = MDDropdownMenu(caller = button, items = button_menu, width_mult = 2)
        self.menu.open()

```

This method is triggered when a button is pressed, initiating a dropdown menu. The dropdown menu is created using the MDDropdownMenu widget from the KivyMD library, with a caller button and a list of menu items defined as dictionaries. Each menu item dictionary specifies text to be displayed, the view class for the item, and an action to be executed when the item is selected, indicated by the on_release event. In this case, the action self.check_material() is triggered with different material types ('glass', 'stainless steel', 'aluminium', 'plastic') as arguments based on the selected menu item. This code segment facilitates user interaction by presenting a dropdown menu for selecting different materials, likely for a specific application feature or setting within the GUI.

## Kivy File: "project3.kv"
### Screen Manager
```.py
ScreenManager:
    id: main_scr
    LoginScreen:
        name: "Login page"

    SignupScreen:
        name: "Signup page"

    ManagerMenu:
        name: "ManagerMenu"

    StaffMenu:
        name: "StaffMenu"

    FinanceScreen:
        name: "FinancePage"

    CustomerScreen:
        name: "CustomerPage"

    OrderScreen:
        name: "OrderPage"

    InventoryScreen:
        name: "InventoryPage"
```
The ScreenManager provides a simple and efficient way to organize and switch between different screens in an application. Each screen is defined using a custom class that inherits from the Screen class, which allows for custom attributes and functionality to be defined for each screen. Abstraction was used to make the process of managing different screens and easily switching between them easier for me.

### MDTextfield
```.py
MDTextField:
            id: username
            size_hint: .8, .15
            pos_hint: {"center_x": .5, "center_y": .5}
            hint_text: "Enter username"
            helper_text: "The username doesn't exist"
            helper_text_mode: "on_error"
            icon_left: "account"
            font_size: "15pt"
```
This widget is assigned the ID username for easy reference within the application code. It is configured with specific size hints, positioning hints to center it on the screen, and appearance properties such as hint text ("Enter username"), helper text ("The username doesn't exist"), and helper text mode ("on_error" mode, indicating it will be displayed when an error occurs). Additionally, it features an icon on the left side of the text field, represented by the "account" icon, serving as a visual cue for the field's purpose. The font size is set to 15pt. Overall, this code segment defines a stylized text input field with visual cues and error feedback, likely intended for users to input their username within the application's interface.

### Encrypting Password
```.py
MDTextField:
            id: cpass
            size_hint: 1, .2
            hint_text: "Enter password again"
            password: True
            helper_text: "The password isn't the same"
            helper_text_mode: "on_error"
            icon_left: "key-chain"
            font_size: "10pt"
```

Here the code creates an MDTextField widget that allows users to input text. The MDTextField is defined with an ID of "cpass" and several attributes such as hint_text, font_size, and password. The hint_text parameter prompts the user with "Enter password again " as placeholder text within the field. The font_size attribute sets the font size of the text within the field to 10 points. The id attribute assigns a unique identifier, "cpas", to the widget, facilitating its reference elsewhere in the application's logic. Finally, the password attribute is set to True. This encrypts the input and provides security and privacy for the users trying to input their password.

### MDBoxLayout
```.py
MDBoxLayout:
        size_hint: .8, .8
        orientation: "vertical"
        pos_hint:{"center_x": .5, "center_y": .5}
        md_bg_color: "white"
        padding: dp(50)

        MDLabel:
            halign: "center"
            id: text
            size_hint: 1, .1
            font_size: "30pt"
            text: "Register"


        MDTextField:
            size_hint: 1, .2
            id: username
            hint_text: "Enter your name"
            helper_text: "The username already exists."
            helper_text_mode: "on_error"
            icon_left: "account"
            font_size: "10pt"
```

MDBoxLayout is utilized to structure the layout of graphical elements. The MDBoxLayout is configured with a size hint of 0.8 by 0.8, making it take up 80% of the available space both horizontally and vertically. It is oriented vertically (orientation: "vertical"), ensuring that its child elements are stacked vertically. Positioned at the center of the screen (pos_hint:{"center_x": .5, "center_y": .5}), it features a white background color (md_bg_color: "white") and padding of 50 density-independent pixels (padding: dp(50)), providing spacing around its contents. Within the MDBoxLayout, there are child elements such as an MDLabel displaying the text "Register" at the top, and an MDTextField below it allowing users to input their name. The MDBoxLayout serves as a container for organizing and arranging these UI elements in a structured and visually appealing manner within the application's interface.


## Criteria D: Functionaliity

### The video 
https://drive.google.com/file/d/1M9zwYsXkGbd7uTwErd3eCURWx87VNIwx/view?usp=drive_link




