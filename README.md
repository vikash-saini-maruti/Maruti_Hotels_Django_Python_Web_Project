# Maruti Hotels Django Python Web Project
----------------------------------------------------------------------------------

This Django project, created by Vikash Saini, aims to provide a platform for hotel management. Users can access the system as either staff or regular users, with an admin portal for managing all aspects of the application. Users can book rooms, check availability by location and date, and view galleries of available luxurious hotels.

## Summury

Maruti Hotels is a Python Django web application designed to streamline hotel management processes. It offers a user-friendly interface for both staff and users to interact with the system efficiently. Users can browse available hotels, book rooms, and check availability based on location and date. The admin portal provides comprehensive management capabilities for overseeing the entire system.


----------------------------------------------------------------------------------


## Features

- User Authentication: Users can sign up, log in, and log out as either staff or regular users.
- Hotel Booking: Users can search for hotels, view available rooms, and book them based on their preferences.
- Admin Portal: Staff members have access to an admin panel for managing hotels, rooms, reservations, and user accounts.
- Room Management: Staff can add, edit, and delete rooms, including details such as room type, capacity, price, and availability.
- Location Management: Staff can add new hotel locations, including details such as city, state, and country.
- Booking Management: Staff can view all bookings, and users can see their booking history.

## Key Points

- **User Roles**: The system supports two user roles: staff and regular users, each with different access privileges.
- **Database Interaction**: The application interacts with a database to store information about hotels, rooms, reservations, and user accounts.
- **Frontend Interface**: The frontend is designed using HTML templates, providing a visually appealing and intuitive user experience.
- **Security**: User authentication is implemented to ensure secure access to the system, with appropriate permissions assigned to each user role.




## Future Improvements

1. **Payment Integration**: Integrate payment gateways to enable online booking and payment processing.
2. **Responsive Design**: Enhance the frontend with responsive design principles to ensure compatibility across various devices.
3. **Advanced Search**: Implement advanced search functionalities, such as filtering rooms by amenities, price range, and ratings.
4. **Review System**: Allow users to leave reviews and ratings for hotels and rooms.
5. **Email Notifications**: Send email notifications to users for booking confirmation, reminders, and updates.

----------------------------------------------------------------------------------

## Installation 

To run the project locally:

1. Clone the repository.
2. Install Python and Django if not already installed.
3. Navigate to the project directory in the terminal.
4. Run `python manage.py runserver` to start the development server.
5. Access the application in a web browser at `http://localhost:8000`.

----------------------------------------------------------------------------------


## Technical Detail

This project is built using Python and the Django web framework. It leverages Django's built-in features for user authentication, database management, and URL routing. The application follows the Model-View-Template (MVT) architecture, where models represent data, views handle user requests, and templates render the HTML output.


### Project Structure
The project follows the typical structure of a Django web application:

- **Models**: Defined in `models.py`, represent the database structure. Models include `Hotels`, `Rooms`, and `Reservation`, which store information about hotels, rooms, and booking reservations, respectively.
- **Views**: Defined in `views.py`, handle user requests and generate responses. Views include functions for rendering HTML templates, processing form data, and managing user authentication.
- **Templates**: HTML templates are stored in the `templates` directory. These templates are used to render the frontend interface and display dynamic content.
- **Static Files**: Static files such as CSS, JavaScript, and images are stored in the `static` directory. These files are used to style the frontend and add interactivity.
- **URLs**: URL patterns are defined in `urls.py`, mapping URLs to corresponding views.
- **Admin Panel**: Django's built-in admin panel (`admin.py`) is used for managing application data.

### Functions in  Detail

#### Import Statements
The `views.py` file begins with import statements, importing necessary modules and classes from Django and the project's own `models`.

#### Function Definitions
1. **Homepage**: Renders the homepage template (`index.html`) and handles hotel search functionality based on user input.
2. **About Page**: Renders the about page template (`about.html`).
3. **Contact Page**: Renders the contact page template (`contact.html`).
4. **User Sign-Up**: Handles user registration form submission, creating new user accounts.
5. **Staff Sign-Up**: Handles staff registration form submission, creating new staff accounts.
6. **User Log-In/Sign-Up Page**: Renders the user login/signup page template and handles user authentication.
7. **Staff Log-In/Sign-Up Page**: Renders the staff login/signup page template and handles staff authentication.
8. **Logout User**: Logs out the current user and redirects to the homepage.
9. **Staff Panel**: Renders the staff panel page template (`staff/panel.html`) and provides staff-specific functionalities.
10. **Edit Room**: Handles room editing form submission by staff members, updating room details.
11. **Add New Room**: Handles adding new room form submission by staff members, creating new room entries.
12. **Book Room Page**: Renders the book room page template (`user/bookroom.html`) and handles room booking functionalities.
13. **Book Room**: Handles room booking form submission, creating new reservation entries.
14. **404 Error Handler**: Renders the custom 404 error page (`404.html`).
15. **View Room**: Renders the view room page template (`staff/viewroom.html`) and displays details about a specific room and its reservations.
16. **User Bookings**: Renders the user bookings page template (`user/mybookings.html`) and displays a user's booking history.
17. **Add New Location**: Handles adding new hotel location form submission by staff members, creating new location entries.
18. **All Bookings**: Renders the all bookings page template (`staff/allbookings.html`) and displays all reservations.

### Technical Overview
- **Database Interaction**: Views interact with the database through Django's ORM (Object-Relational Mapper), querying and manipulating data stored in the database tables.
- **Form Handling**: Views handle form submissions, validate user input, and process data accordingly.
- **User Authentication**: Views manage user authentication, including login, logout, and registration functionalities.
- **Authorization**: Views enforce access control, ensuring that only authenticated users can access certain functionalities.
- **Rendering Templates**: Views render HTML templates, passing dynamic data from the backend to the frontend for display.
- **Error Handling**: Views handle errors, such as 404 errors, by rendering custom error pages for a better user experience.

This detailed overview of the `views.py` file provides insight into how the project handles user interactions, data processing, and rendering of the frontend interface.




