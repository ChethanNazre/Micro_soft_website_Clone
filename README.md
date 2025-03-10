# Micro_soft_website_Clone
A simple and fun Official Microsoft website clone using HTML, Tailwind-CSS

## Tailwind CSS Installation on VS Code

1. **Install Node.js**
   - Download and install Node.js from [nodejs.org](https://nodejs.org/).

2. **Initialize your project**
   - Open your project directory in VS Code.
   - Open the terminal in VS Code (View > Terminal).
   - Run the following commands to initialize your project:
     ```sh
     npm init -y
     ```

3. **Install Tailwind CSS**
   - Run the following command to install Tailwind CSS via npm:
     ```sh
     npm install -D tailwindcss
     ```

4. **Create Tailwind Configuration File**
   - Generate the `tailwind.config.js` file by running:
     ```sh
     npx tailwindcss init
     ```

5. **Configure Tailwind to remove unused styles in production**
   - Update the `tailwind.config.js` file to include your content paths:
     ```js
     module.exports = {
       content: [
         "./src/**/*.{html,js}",
         "./public/index.html",
       ],
       theme: {
         extend: {},
       },
       plugins: [],
     }
     ```

6. **Create your CSS file**
   - Create a `src/styles.css` file and add the following lines:
     ```css
     @tailwind base;
     @tailwind components;
     @tailwind utilities;
     ```

7. **Build your CSS**
   - Add the following scripts to your `package.json` file:
     ```json
     "scripts": {
       "build": "tailwindcss build src/output.css -o src/output.css" ///In this folder styles.css is renamed as output.css
     }
     ```
   - Run the build process:
     ```sh
     npm run build
     ```

## Opening and Executing the Project

1. **Opening the Project**
   - Open your project directory in VS Code.
   - Ensure your file structure includes the `public` directory with `index.html` and `styles.css`.

2. **Executing the Project**
   - Open the `index.html` file in your browser to see the Tailwind CSS styles applied.

## Benefits of Using Tailwind CSS

- **Utility-First**: Tailwind is a utility-first CSS framework which provides low-level utility classes that let you build complex designs without custom CSS.
- **Customization**: It is highly customizable with a configuration file that allows you to tailor it to your needs.
- **Responsive Design**: Tailwind makes it easy to create responsive designs with its pre-built responsive utility classes.
- **Performance**: Tailwind automatically purges unused CSS in production builds, which results in smaller file sizes and better performance.
- **Consistency**: It promotes a consistent design system across your project with its utility-based approach.

## Contact

For any queries, please contact me at chethannazre009@gmail.com
