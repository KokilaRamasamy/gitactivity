Aura Event Planner Website
Title: Aura Event Planner Website
Subtitle: Streamlining Event Management
Kokila Ramasamy &01/14/2025
________________________________________
 Overview
The Aura Event Planner website is a comprehensive platform that simplifies organizing memorable events. It caters to various occasions, including weddings, corporate events, birthdays, and more. With user-friendly features and a visually appealing interface, the website provides a seamless experience for customers to plan and customize their events effortlessly.
Key features include:
•	A visually engaging home page highlighting the services offered.
•	Detailed event type and service pages with stunning visuals and descriptions for catering, decorations, photography, makeup, entertainment, and more.
•	A dynamic invitation page for creating and managing guest invitations.
•	Secure sign-up and login functionality, ensuring personalized access for every user.
•	A robust backend powered by Spring Boot, supporting efficient management of events, services, and user data.
This project aims to revolutionize the event planning experience, blending technology with creativity to deliver unforgettable celebrations.
________________________________________
Architecture
•	Backend: Spring Boot with Hibernate.
•	Frontend: Thyme leaf, HTML, CSS, JavaScript.
•	Database: MySQL.

________________________________________

Pseudocode for Core Functionalities:
1. User Authentication (Sign-Up & Login)
FUNCTION user Authentication()
    IF user selects "Sign-Up":
        INPUT username, email, password
        ENCRYPT password using bcrypt
        SAVE user details in database
        DISPLAY "Registration Successful"
    ELSE IF user selects "Login":
        INPUT username, password
        FETCH user details from database
        VALIDATE encrypted password with user input
        IF valid:
            DISPLAY "Login Successful"
        ELSE:
            DISPLAY "Invalid Credentials"
END FUNCTION
2. Event Planning Workflow
FUNCTION planEvent()
    INPUT eventType (e.g., Wedding, Birthday)
    DISPLAY availableServices based on eventType
    SELECT services (e.g., Catering, Decoration)
    ADD selected services to "Event Cart"
    CALCULATE totalCost based on selected services
    DISPLAY confirmation page
    IF user confirms:
        SAVE event details to database
        DISPLAY "Event Planning Successful"
    ELSE:
        DISPLAY "Event Cancelled"
END FUNCTION
3. Display Service Information
FUNCTION displayServices()
    FETCH serviceDetails from database
    FOR EACH service in serviceDetails:
        DISPLAY serviceName, description, image
    END FOR
END FUNCTION
4. Contact Us Form
FUNCTION submitContactForm()
    INPUT name, email, message
    VALIDATE inputs
    IF valid:
        SAVE message details in database
        SEND acknowledgment email to user
        DISPLAY "Message Sent Successfully"
    ELSE:
        DISPLAY "Invalid Input"
END FUNCTION
________________________________________
Flowchart:
1. User Authentication
 [Start] --> [User Selects Option: Sign-Up or Login]
    --> [Sign-Up?]
        --> [Input Username, Email, Password]
            --> [Encrypt Password]
                --> [Save to Database]
                    --> [Display Success Message]
    --> [Login?]
        --> [Input Username, Password]
            --> [Fetch User Data]
                --> [Validate Credentials]
                    --> [Valid?]
                        --> [Login Success]
                    --> [Invalid]
                        --> [Display Error]
2. Event Planning
 [Start] --> [User Selects Event Type]
    --> [Display Services for Event Type]
        --> [Select Services]
            --> [Add to Cart]
                --> [Calculate Cost]
                    --> [Display Confirmation]
                        --> [User Confirms?]
                            --> [Save Details to Database]
                                --> [Display Success]
                            --> [Cancelled]
                                --> [Display Cancel Message].
________________________________________
Learnings & Future Enhancements
•	Learnings: Improved understanding of Spring Boot, Thyme Leaf, and database integration.
•	Future Enhancements: Add AI-based event suggestions, real-time chat support, and multi-language support.
________________________________________

Conclusion
The purpose of the Aura Event Planner website is to simplify and elevate the event planning process by offering a comprehensive and user-friendly platform. By integrating diverse services such as decoration, catering, photography, and entertainment, the website empowers users to design and execute their dream events seamlessly, whether they're weddings, corporate functions, or private celebrations.
Successful Implementation and Business Use Cases
•	Centralized Event Planning: Users can browse and book services, customize themes, and manage event details in one place, saving time and effort.
•	Enhanced Customer Experience: A visually appealing and intuitive interface ensures a smooth planning journey, encouraging repeat usage and customer satisfaction.
•	Business Integration: Service providers can use the platform to showcase their offerings, reach a wider audience, and grow their business.
•	Scalability: The robust Spring Boot backend and database management ensure the system is scalable for handling multiple concurrent users and large events.
•	Real-World Impact: By addressing common pain points in event planning, such as vendor coordination and budget tracking, Aura Event Planner provides a solution that resonates with customers and service providers.
The successful deployment of this project demonstrates its potential to become a leading tool in the event planning industry, combining innovation, reliability, and creativity.

