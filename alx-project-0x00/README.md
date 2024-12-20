React Genesis: Mastering Next.js Setup
======================================

*    Novice
    
*    Weight: 1
    
*    Project will start Dec 16, 2024 12:00 AM, must end by Dec 23, 2024 12:00 AM
    
*    Checker was released at Dec 16, 2024 12:00 AM
    
*    **Manual QA review must be done** (request it when you are done with the project)
    
*    An auto review will be launched at the deadline
    

### Quiz questions

**Great!** You've completed the quiz successfully! Keep going! (Show quiz)

Tasks
-----

### 0\. Scaffolding a project

**mandatory**

**Objective**: You will understand the essence of creating a project using cli-tools like npx, coupled with create-next-app. There are multiple ways you can create a project using the create-next-app cli-tool.

*   The first approach will be to use the command npx create-next-app@latest This option will provide you with multiple prompts to help set up your initial project
    
*   The next approach is to be familiar with the \[options\] ahead of creating the project. This is the option we will be using.
    

**Instructions**:

*   Start a new visual studio code (vscode instance), open the terminal using the Terminal -> New Terminal
    
*   Navigate to your project directory
    
*   Run the command npx create-next-app@latest alx-project-0x00 –typescript
    
*   Select Yes for the following option \[Eslint, Tailwind CSS, import alias\]
    
*   Select No for /src directory and App Router
    
*   Start your application using the command npm run dev
    

**Repo:**

*   GitHub repository: alx-project-0x00-setup
    
*   Directory: alx-project-0x00
    
*   File: README.md
    

Check submission Get a sandbox

### 1\. Setting up project directories

**mandatory**

**Objective**: Next.js framework provides a better folder structure for your application. Understanding the essence of these projects will help you better organize your assets and components.

**Instructions**:

*   From the root directory, create the following directories components and interfaces
    
*   From the directory pages, open index.tsx and change the named function to an arrow function. Move the export the component at the end of the file.
    

Your code should look like this

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   const Home: React.FC = () => {    return (          Airbnb Application Clone system ===============================        Get Started    )  }  export default Home;   `

*   Create an empty file index.ts in the interfaces directory
    
*   Create an empty file Card.tsx and Pill.tsx in the components directory
    
*   Run npm run dev from the terminal
    
*   From a tab in your browser type http://localhost:3000 to see the changes made.
    

**Repo:**

*   GitHub repository: alx-project-0x00-setup
    
*   Directory: alx-project-0x00
    
*   File: components/Card.tsx, components/Pill.tsx, interfaces/index.ts
    

Check submission

### 2\. Basic Routing

**mandatory**

**Objective**: Next.js provides two types of routing \[App Router and Pages Router\]. You will realize from Task 0, we choose the option \[No\] for App Router. This is because we want to stick to a more simple routing in next.js, In future we will look more into App Router. This task will allow us to explore a simple routing in next.js. This requires no configuration whatsoever.

**Instructions**:

*   You should find a pages/ directory under the root directory. You will find some additional files and folders here.
    
    *   Example: pages/api
        
        *   Index.tsx, \_app.tsx and \_document.tsx
            
*   Remember we already changed the content of the index.tsx. This serves as the entry point for our application when you open http://localhost:3000 in your browser
    
*   Create a new empty file under the pages directory like this:
    
    *   pages/landing.tsx
        
        *   pages/about.tsx
            
*   Open the landing.tsx file and write a basic functional component in there like this.
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   const Landing: React.FC =  () => {    return (                Landing Page ============    )  }  export default Landing   `

*   Open the about.tsx file and write a basic functional component in there like this
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   const About: React.FC =  () => {    return (             About Page ==========    )  }  export default About;   `

*   Run npm run dev from the terminal
    
*   From a tab in your browser type http://localhost:3000/landing to see the changes made.
    
*   From a tab in your browser type http://localhost:3000/about to see the changes made.
    

**Repo:**

*   GitHub repository: alx-project-0x00-setup
    
*   Directory: alx-project-0x00
    
*   File: pages/landing.tsx, pages/about.tsx, interfaces/index.ts, README.md
    

Check submission

### 3\. Rendering Components

**mandatory**

**Objectives**: Building a react application allows developers to identify patterns from their project mockups, design components that can be reusable across one or more pages or event components. This prevents code repetition and leverages on props to make such components dynamic.

*   The components directory we created from previous tasks can be used in this manner. (N:B The name can anything you or your team prefer, but it is advisable to use common standardized names)
    
*   This component can contain a bunch of files related to the components to be worked on or even grouped together under a unified name.
    
*   Components created in this directory can be used in almost every other file in your project. But it is important to use it right
    

**Instructions**:

*   From this Archive (Add link to archive here), move the images \[house.png, star.png\] to public/assets/images
    
*   Navigate to your components folder and open the file card.tsx
    
*   Replace the content with the code below:
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   import Image from "next/image"  import HOUSE_IMAGE from "@/public/assets/house.png"  import STAR_IMAGE from "@/public/assets/star.png"  import React from "react"  import Pill from "./Pill"  const Card: React.FC = () => {   return (              ![house image]({HOUSE_IMAGE})                                ### Villa Arrecife Beach House              Sideman, Bali, Indonesia                      ![star]({STAR_IMAGE})              4.76                                              4                            2                            2-4            $2,450/n    )  }  export default Card   `

*   Navigate to your components folder and open the file pill.tsx
    
*   Replace the content with the code below:
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   const Pill: React.FC = () => {    return (                Title    )  }  export default Pill;   `

*   Run npm run dev from the terminal
    
*   From a tab in your browser type http://localhost:3000/landing to see the changes made.
    
*   This will not show you the component you have just created.
    
*   In the next task, we will explore how to use the components just created
    

**Repo:**

*   GitHub repository: alx-project-0x00-setup
    
*   Directory: alx-project-0x00
    
*   File: components/Card.tsx, components/Pill.tsx, README.md
    

Check submission

### 4\. Using components

**mandatory**

**Objective**: Breaking your application down into components, does not only make you code modular and maintainable, but also speeds up development. Once a component is created it can be used in more than one place. The content of the component can be made dynamic, leverage on powerful features like props, interfaces, and types in typescript. For this task let’s make use of the Card and Pill components we created from the previous task.

**Instructions**: \* From the Card component, we imported and used the Pill Component 3 times. Also, note that we passed an additional prop title, with different strings. Your vscode is properly yelling at you now. Don’t worry we will fix that soon. \* Open pages/landing.tsx \* Add this line of code after your h1 tag

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML

*   At the top of your tsx file include the following import if not done automatically/
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   import Card from "@/components/Card"   `

*   Run npm run dev from the terminal
    
*   From a tab in your browser type http://localhost:3000/landing to see the changes made.
    
*   You should see your card rendered under the h1 tag.
    
*   Duplicate it a couple of times to see how convenient it is to use components.
    

**Repo:**

*   GitHub repository: alx-project-0x00-setup
    
*   Directory: alx-project-0x00
    
*   File: pages/landing.tsx, README.md
    

Check submission

### 5\. Typing your functional components

**mandatory**

**Objective**: Component design can take some getting used to.In your applications and similar other applications, it is important to identify which part of your application can be broken down into smaller components. And how that smaller component can be reused. To reuse a component effectively, we need to make it dynamic by passing some props to that container. \* In Task 4 and 5, We created and used the Pill Component. Note that in Task 4 the Pill component was used in this manner.

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML                         

*   To adjust our pill component to accept the prop “title”, we need to adjust our code a bit.
    

**Instructions**: \* Open interfaces/index.ts \* Add the following code fragment to the file

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   export interface PillProps {    title: string  }   `

*   Remember to save and the file
    
*   Next, open components/pill.tsx
    
*   Include this line at the top of the file
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   import { PillProps } from "@/interfaces";   `

*   Also, modify the functional component to look like this:
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   const Pill: React.FC = ({ title }) => {    return (                {title}    )  }  export default Pill;   `

*   Save and close your files
    
*   Run npm run dev from the terminal
    
*   From a tab in your browser type http://localhost:3000/landing to see the changes made.
    
*   You should see your card rendered under the h1 tag.
    
*   Duplicate it a couple of times to see how convenient it is to use components.
    

**Repo:**

*   GitHub repository: alx-project-0x00-setup
    
*   Directory: alx-project-0x00
    
*   File: interfaces/index.tsx, components/Pill.tsx, README.md
    

Check submission

### 6\. Advanced Task

**mandatory**

**Objective**: Create a button component that accepts title and styles as an argument. Create multiple instances (sizes: small, medium, Large - shapes: rounded-sm, rounded-md, rounded-full) of the button component under the /landing paths.

**Repo:**

*   GitHub repository: alx-project-0x00-setup
    
*   Directory: alx-project-0x00
    
*   File: interfaces/index.tsx, components/Button.tsx, pages/landing.tsx
