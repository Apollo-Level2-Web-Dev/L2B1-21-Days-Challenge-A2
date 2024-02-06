# L2B1 21 Days Challenge NEXT JS Assignment - 2

## Technology Stack:

- Typescript (Recommended. If you want you can use Javascript)
- Next JS
- Next Auth
- Redux (Optional)
- Node-Express (For Backend)
- MongoDB / PostgreSQL
- Mongoose / Prisma / TypeORM / Sequelize(Optional)

## **Project Overview:**

The assignment aims to build a fully functional **Donation Campaign** website using Next.js, following a Figma design and incorporating user authentication, a backend (Node.js Express), and various features:

- Responsive design (At least for Mobile)
- Navigation with active route highlighting
- Banner section with search
- Data fetching from a Database Server
- Card-based UI for donations
- Donation details page with donation confirmation
- User donations page
- Pie chart  statistics page
- **Bonus**:
    - Search functionality by category
    - 20 Meaningful code commits and features in Readme file
    - Custom 404 page
    - Mobile-first development
    - Add an additional Chart Sections (other than Pie Chart) to implement any other statistical data

## **Key Requirements:**

- Use the `app` directory and its routing capabilities.
- Implement user authentication and authorization

<aside>
💡 You can use either NextAuth.JS / Firebase/ OAuth 2.0 or Custom Authentication system in the frontend.

</aside>

- Use Node.js Express for the backend.
- Use Figma design as a guide for UI elements and styling. You can also modify the designs on your own. But the designs should be standard.
- Implement a responsive layout using Tailwind CSS, ShadCn / Ant Design or any similar kind of CSS framework.

## Requirement Analysis:

1. **Backend Integration:**
    - Node.js Express
2. **Database:**
    - You can use **MongoDB / PostgreSQL as Database**. If you are interested, you can use **Mongoose  / Prisma / TypeORM / Sequelize** to create the schema for your database. Keep in mind that **using Mongoose  / Prisma / TypeORM / Sequelize is optional.**
    - **Custom Authentication & Authorization System** in **Backend** to persist the user information like user roles etc.
        
        <aside>
        💡 You can keep JWT token based authentication & authorization or simple authentication without JWT.
        
        </aside>
        
    - In Frontend, Handle User Authentication & Authorization with **Next Auth Credential Provider / Firebase / OAuth 2.0**
        
        <aside>
        💡 If you use Firebase / OAuth 2.0 or Next Auth, you must persist the user information in your database with custom backend.
        
        </aside>
        
    
     ****
    
    <aside>
    💡 You can use any data fetching libraries like **RTK Query / Tanstack Query / React SWR** or if you want you can use the **built in hook of React** to handle the data fetching and authentication / authorization in your frontend
    
    </aside>
    
    - **Create API endpoints to:**
        - Fetch all donations
        - Fetch a single donation by **_id**
        - Create new donations
        - Update donation details
        - Retrieve user donations
        - Calculate donation statistics of each donation
- **User Roles:**
    - **user:**
        - Example User :
            
            ```jsx
            {
              "name": "John Doe",
              "email": "john@gmail.com",
              "password": "123456",
              "role": "user"
              //you can add more fields here on your need.
            }
            ```
            
        - Can view the donation posts
        - Can donate in the donation posts
        - Can see in which donation posts the user has donated *[You can show this in user dashboard]*
    - **admin:**
        - Example Admin :
            
            ```jsx
            {
              "name": "Dave Gray",
              "email": "dave@gmail.com",
              "password": "123456",
              "role": "admin"
              //you can add more fields here on your need.
            }
            ```
            
        - Create/Update/Delete a donation post.
        - Can see the donation statistics of a donation post.
        - Create other admins.
            
            <aside>
            💡 Create the first admin manually in your database.
            
            </aside>
            
1. **Register/Login Page:**
    - Apply your creativity to develop the Register & Login page [These pages are not included in figma]
2. **Navigation and Banner:**
    - Create a `Header` component with the logo, menu items, and active route highlighting.
    - Develop a `Banner` component with title, search bar (bonus), background image, and overlay.
    - Connect the search bar to filter donations by category (optional).
    - Include a Logout Button in the Navbar. Only render it after login and dont show it while logged out.
3. **Cards and Details:**
    - Create a `Card` component for displaying donation information and color customization.
    - Implement dynamic routes (`/donations/[id]`) for donation details pages.
    - Develop a `DonationDetails` page with picture, title, description, and a donation button that displays a success message upon click.
4. **Donations Page:**
    - Create a `Donations` page displaying user donations .
    - Display donations in a grid-based or list-based layout.
    - Include a "See All" button to load more donations if necessary.
    - Make the "View Details" button functional or implement placeholder behavior (optional).
5. **Donation Statistics Page:**
    - Build a `Statistics` page using a library like `react-chartjs-2` to create a pie chart.
    - Calculate donation percentages and display them visually. The pie chart will show your donation and total donation. [Follow the figma file for more detail]
6. **Deployment:**
    - Deploy the application to a suitable hosting platform (Vercel).
    - Handle the 404 Error after page reload
    - Thoroughly test all functionalities, including authentication, donations, navigation, responsiveness, and error handling.

## **Additional Informations:**

- You can implement server actions and mutations to handle data changes and communicate with the frontend.
- Consider using Redux for complex state management if needed.
- Adhere to best practices for code structure, naming conventions, and comments for clarity and maintainability.
- Structure your code into reusable components for maintainability.
- Use clear and descriptive variable and function names
- Consider implementing server-side rendering (SSR) or static site generation (SSG) where possible for better SEO and performance.

## **Deadline:**

- 60 marks: February 10, 2024 11.59 PM
    
    <aside>
    💡 There is no 50 / 30 Marks Deadline.
    
    </aside>
    

## Important Note:

Plagiarism will not be tolerated. Ensure that the code you submit is your own work. Any instances of plagiarism will result in 0 Marks.

Good luck with your assignment! If you have any questions, feel free to reach out for clarification.