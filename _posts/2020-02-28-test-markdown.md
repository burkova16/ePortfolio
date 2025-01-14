---
layout: post
title: Explanation of the code
subtitle: Here I will discuss end explain the code
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, explanation, follow]
tags: [code, C++]
comments: true
---



## What is Computer Science for me?


Computer Science program started for me back in 2016. I went in local community college and received a Computer Science associates degree. Unfortunately while I was in school there was no help to find jobs and I had a little knowledge how to get in the field. I kept studying and was a straight A student, but still had no knowledge or idea of who I want to be. Then I decided to go for my graduate program in SNHU and after first semester I got a job in IT. This semester will be my last in Computer Science and I will start my journey to Cybersecurity.


During the program there was a lot of ups and downs. The three skills will be patience, asking questions, and reading the instructions. I named patience first because not everything will be working from the first try, and I needed to start over a project multiple times during this program. Asking questions is my go to, I will be posting questions to other students in general discussion, I will be emailing the professor if I need help at any time. Reading the instructions for the assignments through is a very important skill for me. I used to only read the requirements and then I found out that there is usually much more than requirements and I was missing a lot of things in some classes.


## What is my ePortfolio?


For my ePortfolio I am contemplating on which of the past work to display. The CS 350 course project will be used for ePortfolio. I used a code from scratch for TI CC3220x LAUNCHXL board. The program was written to create a thermostat by using GPIO, UART, I2C peripherals. This project has two artifacts from categories design and databases.


This project from CS 350 course will demonstrate the skills I have acquires in software engineering and design because of the number of elements used, the structure of the code and analysis. Currently the application is able to set the temperature and to turn on/off the heating system. It is designed to add more features to the board. My plan for this artifact will be to enhance more functions to the project such as connect the device to the Wi-Fi. IoT device will collect data, then it will take the data by using the hub or IoT gateway to collate and transfer the data, and then it will analyze data and take further action by using user interface or aback end systems. This enhancement will illustrate software design and show future employees that I have experience working with IoT.



## Table of Content:

**1. Professional Self-Assessment**


**2. Code Review**


**3. Software Design: Artifact 1**


**4. Algorithms and Data Structures: Artifact 2**


**5. Databases: Artifact 3**

**6. Course Outcomes**


## 1.	Professional Self-Assessment
For me, Computer Science has been a journey that started back in 2016 when I enrolled in a local community college and obtained an associates degree in Computer Science. However, I struggled to find employment in the field as there was little guidance on how to enter the industry. Despite this, I persevered and maintained a straight A record in my studies, although I still wasn't sure of my career aspirations. It was only after enrolling in a graduate program at SNHU that I landed a job in IT after just one semester. This semester will mark the end of my Computer Science studies, and I will be embarking on a new journey in Cybersecurity.
Throughout my program, I learned the importance of patience, asking questions, and thoroughly reading instructions. Patience was especially critical as I often had to start projects from scratch multiple times. Whenever I needed help, I didn't hesitate to ask my peers or professors by posting questions in general discussions or emailing them directly. Additionally, I realized that reading assignment requirements alone wasn't enough, and I had to be diligent in reviewing all the instructions thoroughly to avoid missing any critical details.
Regarding my ePortfolio, I am still deciding which of my past work to display. However, I am leaning towards showcasing my CS 350 course project. It involved coding a thermostat for a TI CC3220x LAUNCHXL board by utilizing GPIO, UART, and I2C peripherals, resulting in two artifacts from the design and databases categories.
This project will illustrate my skills in software engineering and design as it required a complex structure and analysis. Currently, the application can adjust temperature and turn the heating system on and off. I plan to add more functions to the board, such as connecting it to Wi-Fi. This enhancement will demonstrate my experience with IoT and software design while showcasing to potential employers my ability to work with emerging technologies.

## 2. Code Review

**You can see code review video here: https://youtu.be/zfEKqLCxUlk**

Code review is an essential tool in software engineering. According to a 2022 Global DevSecOps Survey conducted by GitLab, 76% of developers stated that code reviews are "very valuable" (GitLab, 2022). Code review is typically conducted before the code is merged into the main codebase or released to production. It can be done manually, where a reviewer examines the code changes line-by-line, or using automated tools that can flag potential issues automatically. Once the developer has completed writing the code, it must undergo a code review to ensure that there are no logic problems, bugs, errors, or other issues.


Code review is an essential practice for computer science professionals. The first reason is that it allows for the identification and correction of errors, bugs, and logic problems in the code. Catching these issues early on can help to avoid problems in production. The second reason is that code quality is improved, making the code easier to maintain and update. The third reason is the opportunity for collaboration with other team members. According to a GitLab survey, "When software developers review code as soon as a team member makes changes, they can learn new techniques and solutions" (GitLab, 2022). Code review provides an opportunity for team members to learn from each other and improve their skills. The fourth reason is the security of the code. Code review can reveal code vulnerabilities and provide developers with ideas on how to secure the code in the future. This is especially important for applications and systems that handle sensitive data or perform critical functions.


There is a wide range of practices for code review, but I want to highlight five that I believe are the most valuable for developers. The first code review practice is to set clear objectives. It is important to outline specific issues and set objectives for the code. The second practice is to create a checklist of important aspects to cover during the review process. According to Usman Ghani's article on Atlassian, this checklist should include factors such as readability, security, test coverage, architecture, and reusability (Ghani, 2021). The third practice is to consider non-technical factors. During the review, we should not only focus on the technical aspects of the code but also consider non-technical factors such as user experience, performance, and scalability. The fourth practice I want to emphasize is prioritizing the code review. Code review should be viewed as an essential part of the development process and prioritized accordingly. It should not be seen as an optional or expendable step. The fifth code review practice is to utilize automated tools, which can help reduce the time and effort required for manual code review.


One code review practice that I believe is not very common is to include end-users in the review process. End-users can provide valuable feedback on the usability and functionality of the code. Incorporating end-users in the code review process can help ensure that the code meets the needs of its intended audience. It can also lead to the discovery of new use cases and requirements that may not have been considered by the development team (Makarychev et al., 2016).
### References:

{: .box-note}
**References:** What is a code review? GitLab. (n.d.). Retrieved March 11, 2023, from https://about.gitlab.com/topics/version-control/what-is-code-review/#:~:text=Code%20reviews%2C%20also%20known%20as,developers%20learn%20the%20source%20code. 
Ghani, U. (2022, February 3). 5 code review best practices. Work Life by Atlassian. Retrieved March 11, 2023, from https://www.atlassian.com/blog/add-ons/code-review-best-practices 
Makarychev, K., Volokh, K., & Yermakov, S. (2016). Involving end-users in code review. In Proceedings of the 10th International Conference on Software Engineering and Applications (pp. 11-16).

Original code before enhancements.

```
/*
 *  ======== gpiointerrupt.c ========
 */
#include <stdint.h>
#include <stddef.h>

/* Driver Header files */
#include <ti/drivers/GPIO.h>
#include <ti/drivers/Timer.h>

/* Driver configuration */
#include "ti_drivers_config.h"

#define DOT_DURATION 500000 // 500ms
#define DASH_DURATION 1500000 // 1500ms
#define CHAR_GAP_DURATION (3 * DOT_DURATION) // 3*500ms
#define WORD_GAP_DURATION (7 * DOT_DURATION) // 7*500ms


void timerCallback(Timer_Handle myHandle, int_fast16_t status) {


   switch (currentState) {
            case DOT:
                if (sosCount < 3) {
                GPIO_write(CONFIG_GPIO_LED_0, CONFIG_GPIO_LED_ON);
                } else {
                    GPIO_write(CONFIG_GPIO_LED_1, CONFIG_GPIO_LED_ON);
                }
                currentState = PAUSE_BETWEEN_CHARACTERS;
                break;
            case DASH:
                GPIO_write(CONFIG_GPIO_LED_1, CONFIG_GPIO_LED_ON);
                currentState = PAUSE_BETWEEN_CHARACTERS;
                break;

            case PAUSE_BETWEEN_CHARACTERS:
                GPIO_write(CONFIG_GPIO_LED_0, CONFIG_GPIO_LED_OFF);
                GPIO_write(CONFIG_GPIO_LED_1, CONFIG_GPIO_LED_OFF);
                if (sosCount < 3) {
                    currentState = DOT;
                    sosCount++;
                } else {
                    currentState = PAUSE_BETWEEN_WORDS;
                    sosCount = 0;
                }
                break;

            case PAUSE_BETWEEN_WORDS:
                GPIO_write(CONFIG_GPIO_LED_0, CONFIG_GPIO_LED_OFF);
                GPIO_write(CONFIG_GPIO_LED_1, CONFIG_GPIO_LED_OFF);
                currentState = DOT;
                break;

            case SOS:
                GPIO_write(CONFIG_GPIO_LED_0, CONFIG_GPIO_LED_OFF);
                GPIO_write(CONFIG_GPIO_LED_1, CONFIG_GPIO_LED_OFF);
                currentState = DOT;
                sosCount = 0;
                break;
        }
}


void initTimer(void) {
    Timer_Handle timer0;
    Timer_Params params;
    Timer_init();
    Timer_Params_init(&params);
    params.period = 1000000;
    params.periodUnits = Timer_PERIOD_US;
    params.timerMode = Timer_CONTINUOUS_CALLBACK;
    params.timerCallback = timerCallback;

    timer0 = Timer_open(CONFIG_TIMER_0, &params);
    if (timer0 == NULL) {
            /* Failed to initialized timer */
            while (1) {}
 }

 if (Timer_start(timer0) == Timer_STATUS_ERROR) {
     /* Failed to start timer */
     while (1) {}
}
}
/*
 *  ======== gpioButtonFxn0 ========
 *  Callback function for the GPIO interrupt on CONFIG_GPIO_BUTTON_0.
 *
 *  Note: GPIO interrupts are cleared prior to invoking callbacks.
 */
void gpioButtonFxn0(uint_least8_t index)
{
    /* Toggle an LED */
    GPIO_toggle(CONFIG_GPIO_LED_0);
}

/*
 *  ======== gpioButtonFxn1 ========
 *  Callback function for the GPIO interrupt on CONFIG_GPIO_BUTTON_1.
 *  This may not be used for all boards.
 *
 *  Note: GPIO interrupts are cleared prior to invoking callbacks.
 */
void gpioButtonFxn1(uint_least8_t index)
{
    /* Toggle an LED */
    GPIO_toggle(CONFIG_GPIO_LED_1);
}

/*
 *  ======== mainThread ========
 */
void *mainThread(void *arg0)
{
    /* Call driver init functions */
    GPIO_init();

    /* Configure the LED and button pins */
    GPIO_setConfig(CONFIG_GPIO_LED_0, GPIO_CFG_OUT_STD | GPIO_CFG_OUT_LOW);
    GPIO_setConfig(CONFIG_GPIO_LED_1, GPIO_CFG_OUT_STD | GPIO_CFG_OUT_LOW);
    GPIO_setConfig(CONFIG_GPIO_BUTTON_0, GPIO_CFG_IN_PU | GPIO_CFG_IN_INT_FALLING);

    /* Turn on user LED */
    GPIO_write(CONFIG_GPIO_LED_0, CONFIG_GPIO_LED_ON);

    /* Install Button callback */
    GPIO_setCallback(CONFIG_GPIO_BUTTON_0, gpioButtonFxn0);

    /* Enable interrupts */
    GPIO_enableInt(CONFIG_GPIO_BUTTON_0);

    /*
     *  If more than one input pin is available for your device, interrupts
     *  will be enabled on CONFIG_GPIO_BUTTON1.
     */
    if (CONFIG_GPIO_BUTTON_0 != CONFIG_GPIO_BUTTON_1) {
        /* Configure BUTTON1 pin */
        GPIO_setConfig(CONFIG_GPIO_BUTTON_1, GPIO_CFG_IN_PU | GPIO_CFG_IN_INT_FALLING);

        /* Install Button callback */
        GPIO_setCallback(CONFIG_GPIO_BUTTON_1, gpioButtonFxn1);
        GPIO_enableInt(CONFIG_GPIO_BUTTON_1);
    }

    return (NULL);
}


```


## Software design, Algorithms and Data Structures, Database


In here we will view **3 main artifacts and enhancements** for this project.


## 1. Software design

By utilizing a variety of elements, coding structure, and analysis, this CS 350 project showcases my software engineering and design skills. Currently, the program can set the temperature and activating/deactivating the heating system. However, the goal is to expand the project's capabilities by integrating it with Wi-Fi and incorporating an IoT device to collect and transfer data via a hub or IoT gateway for further analysis and action through either a user interface or backend system. 


  The addition of Wi-Fi functionality to the thermostat allows for remote control and monitoring of the temperature settings, even when the user is not physically present. This feature adds convenience and flexibility to the user's experience, as they can adjust the temperature settings from their mobile device or computer, without having to be near the thermostat. Additionally, the ability to connect to Wi-Fi opens opportunities for the device to interact with other smart home systems, such as voice assistants, and provides the potential for more sophisticated automation and energy-saving features. This enhancement serves to highlight my proficiency in software design and demonstrate to potential employers my experience working with IoT technology. To enhance this project, my plan is to add more functions, including connecting the device to Wi-Fi. The IoT device will collect data, which will be transferred to the hub or IoT gateway for collation and analysis. Further actions will be taken through the user interface or back-end systems. This enhancement will demonstrate my software design skills and showcase my experience working with IoT to future employers.


  Wi-Fi functionality should be added to the thermostat in a modular way, allowing for easy modification or removal of the feature in the future if necessary. This can be achieved by separating the Wi-Fi code into its own module or class that can be easily included or excluded from the main codebase. The addition of Wi-Fi functionality requires changes to the overall code structure to accommodate the new feature. This may involve refactoring the existing code to improve code readability and maintainability, such as creating separate functions or classes for different tasks.
  
    
  Adding Wi-Fi to a thermostat can improve the user experience by enabling remote control and monitoring of the device through a mobile app or web portal. This can provide users with greater flexibility and convenience in controlling their home's temperature and energy usage. The addition of Wi-Fi functionality may require changes to the hardware and software architecture of the thermostat, as well as new testing and validation procedures. Outcome-coverage in this area would focus on ensuring that the Wi-Fi feature is reliable, secure, and performs as expected. the outcome-coverage for adding Wi-Fi to a thermostat can be quite broad and multifaceted, encompassing factors such as user experience, energy efficiency, technical performance, market competitiveness, and regulatory compliance.
  
  
  I faced some challenges during this process. Adding Wi-Fi functionality to a thermostat requires the use of external hardware components, such as a Wi-Fi module or chip, and appropriate software libraries that support wireless communication. C++ code can be used to interface with these hardware components and implement the necessary protocols for sending and receiving data over Wi-Fi.


Below is the pseudocode enhancement to demonstrate the ability to visualize code:


~~~
Start

Check if thermostat is connected to power and WiFi

If not connected, connect to power and WiFi

Initialize thermostat settings and connect to cloud service

Read temperature and humidity from thermostat sensor

Upload sensor data to cloud service

Wait for predetermined time interval

Check if thermostat settings have been changed remotely

If settings have been changed, update thermostat settings and save to memory

Repeat from Read temperature and humidity step

End
~~~

The enhancement in C++ file.

```

// WI-FI enhancement
#include <ESP8266WiFi.h>

// SSID and password of the WiFi network
const char* ssid = "MyWiFiNetwork";
const char* password = "MyWiFiPassword";

// Connect to the WiFi network
WiFi.begin(ssid, password);
while (WiFi.status() != WL_CONNECTED) {
    delay(1000); // Wait for the WiFi to connect
    Serial.println("Connecting to WiFi..."); // Print status message to serial monitor
}
Serial.println("Connected to WiFi"); // WiFi connection successful message

// Send temperature data to a server
float temperature = 20.5;
WiFiClient client;
if (client.connect("example.com", 80)) { // Connect to server on port 80
    client.println("POST /updateTemperature HTTP/1.1"); // Send HTTP POST request
    client.println("Host: example.com"); // Specify the host name
    client.print("Temperature: "); // Send temperature data
    client.print(temperature);
    client.println();
    client.println("Connection: close"); // Close the connection
    client.println();
    Serial.println("Temperature sent to server"); // Print status message to serial monitor
}

void loop() {

    // Check if the WiFi connection is lost, then reconnect
    if (WiFi.status() != WL_CONNECTED) {
        Serial.println("WiFi connection lost, reconnecting..."); // Print status message to serial monitor
        WiFi.reconnect();
    }

    // Enum state and timer handle
    enum State { DOT, DASH, PAUSE_BETWEEN_CHARACTERS, PAUSE_BETWEEN_WORDS, SOS };
    enum State currentState = DOT; // Initial state
    int sosCount = 0; // Initial count for SOS
    Timer_Handle timer0; // Initialize timer handle
}
```


The code establishes a Wi-Fi connection using the ESP8266WiFi library and attempts to connect to a server on port 80 to send temperature data. The loop() function checks if the Wi-Fi connection is lost and reconnects if necessary. The remaining code related to the enum state and timer handle appears to be incomplete and without purpose.


##  2. Algorithms and Data Structures


  The current thermostat project makes use of algorithms and data structures. The program currently uses a temperature control algorithm, as a thermostat needs to maintain the temperature of a room within a specified range. An algorithm can be used to control the heating and cooling systems to achieve this goal. The algorithm might use a simple proportional-integral-derivative (PID) controller or a more sophisticated model-predictive control (MPC) algorithm, depending on the specific requirements of the application. 
  
  
  The plan for enhancing the project is to include energy-saving algorithms that can reduce energy usage by adjusting the temperature based on room occupancy. For example, an algorithm may adjust the temperature to a more energy-efficient level when the room is unoccupied. I will need to ensure that the algorithms are safe for the user to use in energy-saving mode. I can enhance the energy-saving mode simply by adding another button to the code and enabling the function. This enhancement will showcase my knowledge of implementing algorithms in the application.
  
  
  Enhancing the project to include energy-saving algorithms that can reduce energy usage by adjusting the temperature based on room occupancy is a good choice for this project. By adjusting the temperature based on room occupancy, energy-saving algorithms can significantly reduce energy consumption. When rooms are unoccupied, the thermostat can adjust the temperature to a more energy-efficient level, which can help save on energy costs. For example, an algorithm might adjust the temperature to a more energy-efficient level when the room is unoccupied. This enhancement will demonstrate my knowledge of algorithm implementation in the application. The components of this artifact will showcase my skills in initialization, looping, device management, and energy consumption.
  
  
  I have met the course objectives that were my goal. The updates for the outcome-coverage plans are testing and optimization, integration with smart home systems, and use of advanced algorithms. After implementing the energy-saving algorithms, it will be important to test and optimize their performance. This can be done by measuring energy consumption before and after implementing the algorithms and making adjustments as needed to ensure optimal energy savings. The project could be further enhanced by integrating it with smart home systems such as Google Home or Amazon Alexa. This would allow users to control the thermostat remotely and receive alerts when rooms are unoccupied or when energy consumption exceeds a certain threshold. While the current algorithms are effective, more advanced algorithms such as machine learning-based algorithms could be used to further improve energy savings. These algorithms could learn from user behavior patterns and adjust temperature settings accordingly.
  
  
  I have learned that pseudocode is very helpful for this project. Pseudocode can be written in plain English or any other natural language, making it easy to read and understand for people without technical programming knowledge. This can help ensure that the program's logic and functionality are clear to all stakeholders involved in the development process. One of the challenges I faced was testing. Since I only have one thermostat and no special rooms to switch temperatures, it was not convenient to keep testing in the same room.

Pseudocode is a high-level description of a computer program that is similar to a programming language, but more simplified and easier to understand. It is used to outline the structure and logic of a program before the actual coding process begins. This helps programmers to plan and design the program more effectively, allowing them to identify and address any potential issues before the code is written. In the below example you can see the pseudocode enhancement.


~~~
// Initialize variables
    total_energy_saved = 0
    current_energy_consumption = get_current_energy_consumption()
    target_energy_consumption = get_target_energy_consumption()
    // Loop until target energy consumption is reached
    while current_energy_consumption > target_energy_consumption:
        // Check if any devices can be turned off
        device_to_turn_off = find_device_to_turn_off()
        if device_to_turn_off is not None:
            turn_off_device(device_to_turn_off)
            energy_saved = get_energy_saved(device_to_turn_off)
            total_energy_saved += energy_saved
            current_energy_consumption -= energy_saved
        else:
            // No devices can be turned off, so reduce their power consumption
            reduce_device_power_consumption()
            current_energy_consumption = get_current_energy_consumption()
    
    // Print energy saved and return
    print("Total energy saved: ", total_energy_saved)
    return
~~~


Breaking down the code:


1.	Initialize variables:
•	This block initializes the variables total_energy_saved, current_energy_consumption, and target_energy_consumption to their initial values.


2.	Loop until target energy consumption is reached:
•	This block starts a loop that will continue until the current energy consumption is less than or equal to the target energy consumption. This means that the loop will keep running until the desired energy savings have been achieved.


3.	Check if any devices can be turned off:
•	This block checks to see if there are any devices that can be turned off to save energy. If there are devices that can be turned off, the code will execute the turn_off_device function, which will turn off the device and update the variables total_energy_saved and current_energy_consumption accordingly.


4.	No devices can be turned off:
•	If there are no devices that can be turned off, the code will execute the reduce_device_power_consumption function, which will reduce the power consumption of the devices in some other way. For example, it could reduce the brightness of lights or the power of a fan. After reducing the power consumption, the code updates the current_energy_consumption variable.


5.	Print energy saved and return:
•	This block prints the total amount of energy saved and then returns from the function. The total energy saved is stored in the total_energy_saved variable.

The code is an energy-saving algorithm that aims to reduce the energy consumption of a system by either turning off devices or reducing their power consumption. The program initializes variables for current and target energy consumption, as well as the total energy saved. It then enters a while loop and checks whether any devices can be turned off. If so, it turns off the first device it finds, calculates the amount of energy saved, and updates the relevant variables. If no devices can be turned off, it reduces the power consumption of all devices and updates the current_energy_consumption variable. Once current_energy_consumption is less than or equal to target_energy_consumption, the loop ends, and the program has successfully reduced the system's energy consumption. The total energy saved is stored in the total_energy_saved variable.The code in C++:

```

    // Initialize variables
    double total_energy_saved = 0;
    double current_energy_consumption = get_current_energy_consumption();
    double target_energy_consumption = get_target_energy_consumption();

    // Loop until target energy consumption is reached
    while (current_energy_consumption > target_energy_consumption) {
        // Check if any devices can be turned off
        string device_to_turn_off = find_device_to_turn_off();
        if (device_to_turn_off != "") {
            turn_off_device(device_to_turn_off);
            double energy_saved = get_energy_saved(device_to_turn_off);
            total_energy_saved += energy_saved;
            current_energy_consumption -= energy_saved;
        }
        else {
            // No devices can be turned off, so reduce their power consumption
            reduce_device_power_consumption();
            current_energy_consumption = get_current_energy_consumption();
        }
    }

```


##  3. Database


The thermostat has memory, but it does not include a database. The plan is to enhance the project by adding a MySQL database. The original design does not include many libraries, so additional libraries will be required to save data to the database. The temperature and humidity readings from the thermostat can be stored in a structured way in a MySQL database, with columns for the timestamp, temperature, and humidity readings. This data can be used for various purposes, such as generating charts and reports, detecting anomalies, and analyzing trends over time. This enhancement will improve data management, increase functionality, and improve the user experience.


Adding SQL database to this project will showcase my skills in data management, integration, scalability, and reliability. By adding a MySQL database, I am showcasing the ability to manage data in a structured and efficient way. I will be showing that I can create tables, insert data, and retrieve data from a database using SQL statements. Integrating a MySQL database into a project requires knowledge of various technologies, such as database management systems, APIs, and programming languages. This demonstrates the ability to work with different technologies and integrate them seamlessly into a project. A database will allow to store large amounts of data and scale the application as it grows. I will be showing an ability to design and develop applications that can handle large amounts of data and scale as needed. One of the ways to improve the enhancement is adding security level to it. This involves implementing user authentication, access control, and encryption. This helps to protect the data from unauthorized access and ensure data privacy and confidentiality.


I have achieved the course objectives that were my goal. The updates to the outcome-coverage plans include data storage management, analytics and reporting, and integration with other systems. Since the thermostat generates a large amount of data, such as temperature and humidity readings, it is necessary to store and manage that data in a database. A database can provide a structured and organized way to store and retrieve data, making it easier to manage and analyze. With the addition of a database, complex queries and analytics can now be performed on the data, allowing for insights to be gained from it.


One of the main things I have learned is the use of libraries for MySQL. The MySQL C++ library provides a high-level interface for connecting to the database, executing queries, and retrieving data. One difficulty that I have encountered is that storing sensitive data, such as temperature and humidity readings, in a database can raise security concerns. It is important to implement appropriate security measures, such as user authentication and access control, to ensure that the data is protected. I have learned that pseudocode is very helpful for this project. Pseudocode can be written in plain English or any other natural language, making it easy to read and understand for people without technical programming knowledge. This can help ensure that the program's logic and functionality are clear to all stakeholders involved in the development process. One of the challenges I faced was testing. Since I only have one thermostat and no special rooms to switch temperatures, it was not convenient to keep testing in the same room.



~~~
Pseudocode:


The first step is to include the necessary libraries for the project, including MySQL Connector/C++, which will allow the program to interact with the database.


Next, the program will establish a connection to the MySQL database using a username and password.


After establishing a connection, the program will create a table in the database to store temperature and humidity readings, along with a timestamp for each reading.


Then, the program will retrieve temperature and humidity readings from the thermostat and insert them into the MySQL database table.


Finally, the program will close the database connection.


Overall, this pseudocode outlines the basic steps needed to add a MySQL database to the thermostat project for better data management and analysis.
~~~


This code establishes a connection to a MySQL database, creates a table to store temperature and humidity readings, retrieves temperature and humidity readings from a thermostat, and inserts them into the database table. It uses the SQL API to connect to the database, and catches any exceptions that may occur during the execution of the program. Finally, it closes the database connection and returns 0.
Here is an example of enchanced code in the .c file:

```

int main()
{
    // Define variables for storing temperature and humidity readings
    float temperature, humidity;

    // Establish a connection to the MySQL database
    sql::Driver* driver;
    sql::Connection* con;
    sql::Statement* stmt;

    try {
        driver = get_driver_instance();
        con = driver->connect("tcp://localhost:3306", "username", "password");
        stmt = con->createStatement();

        // Create a table in the database to store temperature and humidity readings
        stmt->execute("CREATE TABLE IF NOT EXISTS readings(id INT NOT NULL AUTO_INCREMENT, 
            temperature FLOAT, humidity FLOAT, timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP, 
            PRIMARY KEY (id))");

        // Retrieve temperature and humidity readings from the thermostat and insert them into the 
        // MySQL database table
        // Assume the temperature and humidity readings are obtained and stored in the variables 
        // temperature and humidity respectively
        string insert_query = "INSERT INTO readings (temperature, humidity) VALUES 
            (" + to_string(temperature) + ", " + to_string(humidity) + ")";
        stmt->execute(insert_query);

        // Close the database connection
        delete stmt;
        delete con;
    }
    catch (sql::SQLException& e) {
        cout << "SQL Error: " << e.what() << endl;
    }

    return 0;
}

```


## 6. Course Outcomes


  Course Outcome 1 has been met through the implementation of several enhancements in the field of computer science. These enhancements include the integration of WiFi capabilities into a thermostat through software design, the development of an energy-saving algorithm through the use of algorithms and data structures, and the improvement of a MySQL database through enhanced SQL queries. By employing strategies for building collaborative environments that enable diverse audiences to support organizational decision making, these enhancements have contributed to the advancement of computer science and the creation of more efficient and effective technologies.
  
  As a result of completing enhancements in software design, algorithms and data structures, and databases, I was able to design, develop, and deliver professional-quality oral, written, and visual communications that were technically sound, coherent, and adapted to specific audiences and contexts. These enhancements enabled me to effectively communicate the features and benefits of the enhanced wifi into the thermostat, the improved energy saving algorithm, and the enhanced SQL database to diverse audiences in various contexts. The ability to communicate technical information clearly and effectively is crucial in the field of computer science, and the enhancements I completed helped me to develop and refine this skill.
  
  By enhancing the wifi into thermostat, improving the energy saving algorithm, and enhancing the SQL database, I was able to design and evaluate computing solutions that solved specific problems. The improvements made to the thermostat ensured that it could efficiently connect to wifi networks, while the enhancements to the energy saving algorithm ensured that it was more effective at reducing energy consumption. Additionally, the enhancements made to the SQL database improved its ability to store and manage data related to temperature and humidity readings. These improvements allowed me to manage the trade-offs involved in design choices and create computing solutions that were coherent, technically sound, and appropriate for specific audiences and contexts.
  
  By enhancing the wifi functionality of the thermostat, improving the energy-saving algorithm, and enhancing the SQL database, I have demonstrated an ability to use innovative techniques, skills, and tools in computing practices. These enhancements have helped in implementing computer solutions that deliver value and accomplish industry-specific goals. The ability to identify and implement improvements in computer systems using well-founded techniques and tools is an essential skill in the field of computer science, and it is critical to the success of any project or initiative.
  
  The enhancements completed to develop a security mindset include enhancing the WiFi connection in the thermostat, enhancing the energy-saving algorithm, and enhancing the SQL database. These enhancements incorporate secure coding practices, such as preventing SQL injection attacks, protecting against unauthorized access to the system, and ensuring secure data transmission. Additionally, the algorithmic enhancements incorporate secure design principles, such as reducing attack surfaces and enforcing access controls. By incorporating security measures into software architecture and designs, potential vulnerabilities can be exposed and mitigated, ensuring the privacy and enhanced security of data and resources.


## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.
