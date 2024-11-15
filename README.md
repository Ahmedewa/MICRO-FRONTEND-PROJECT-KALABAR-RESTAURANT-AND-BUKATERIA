# MICRO-FRONTEND-PROJECT-KALABAR-RESTAURANT-AND-BUKATERIA
TITLE-MICRO FRONTEND PROJECT-KALABAR RESTAURANT AND BUKATERIA

              READ.ME
A)AIMS AND GOALS OF THE PROJECT

B)PREREQUISITES/CONTENTS:
1).DEVELOPMENT ENVIRONMENT.
Download Node.js
Download React application

IDEs: VSCode, Vim, Jupyter Notebook, Notepad++, Angular, PyCharm

Tools and Frame Works
-Webpack
-Angular
-React
-Vuej.s
-Webpack Module Federation
-Single-Spa

2)MEDIA:
-Diagrams (Flow charts)
-Videos
3).CODE:

4).DEBBUGGING:
-Debugging Technique.

5).COMMON PITFALLS/PROBLEMS:

6).CONCLUSION:

         DESCRIPTION/GOALS OF THE PROJECT
The project is a MICRO MONO-FRONTEND PROJECT-'KALABAR RESTAURANT AND BUKATERIA'-Using the ANGULAR Framework.
kalabar(Calabar- a town in Southeastern,Nigeria,Capital of Cross River State). 
Popular for its Culinary Excellence , especially noted for :Afang Soup ,Edikaikong Soup,and Afia Efere(White Soup-Made From Pounded Yam Water), and Fufu(Made from Processed Cassava-Manioc).
This forms the 'Menu' of 'KALABAR RESTAURANT AND BUKERTERIA'.


                CODE
The code is broken down from a Single -Monolithic Structure(Shell Package/Bundle) into Smaller Packets namely:
1)Email Component (Module).
2)Menu Component(Module).
3)Order Component(Module).
4)Payment Component(Module).
5)Location(Module).
6)Delivery Component(Module).
All of the above is done using ANGULAR(A Java Script framework developed by Google.)
It uses TypeScript,HTML,and CSS Code.
-Typescript:is used by ANGULAR as its Primary Programming Language.
-HTML:is used by ANGULAR as its Template Language.
-CSS:is used by ANGULAR for styling and Layout purposes.



HTML CODE 

<!DOCTYPE html>
<html style="font-size: 10px; font-family: Roboto, Arial, sans-serif;">
  <head>
    <title>Kalabar Restaurant and Bukerteria</title>
    < (Angular  scripts) 
  </head>
  <body dir="ltr" rounded-container data-new-gr-c-s-loaded="14.1089.0">
    <app-root></app-root>
    <grammarly-desktop-integration data-grammarly-shadow-root="true"></grammarly-desktop-integration>
  </body>
</html>



CSS CODE

:root {
  --primary-color: #3f51b5;
  --light-primary-color: #c5cae9;
  --dark-primary-color: #303f9f;
  --accent-color: #ff4081;
  --light-accent-color: #ff80ab;
  --dark-accent-color: #f50057;
  --light-theme-background-color: #fff;
  --light-theme-base-color: #000;
  --light-theme-text-color: #212121;
  --light-theme-secondary-color: #737373;
  --light-theme-disabled-color: #9b9b9b;
  --light-theme-divider-color: #e0e0e0;
  --dark-theme-background-color: #212121;
  --dark-theme-base-color: #000;
  --dark-theme-text-color: #fff;
  --dark-theme-secondary-color: #bdbdbd;
  --dark-theme-disabled-color: #646464;
  --dark-theme-divider-color: #424242;
}


ANGULAR CODE STRUCTURE
app.module.ts


TYPE SCRIPT

import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent } from './app.component';
import { EmailComponent } from './email/email.component';
import { OrderComponent } from './order/order.component';
import { MenuComponent } from './menu/menu.component';
import { PaymentComponent } from './payment/payment.component';
import { LocationComponent } from './location/location.component';
import { DeliveryComponent } from './delivery/delivery.component';

@NgModule({
  declarations: [
    AppComponent,
    EmailComponent,
    OrderComponent,
    MenuComponent,
    PaymentComponent,
    LocationComponent,
    DeliveryComponent
  ],
  imports: [
    BrowserModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }




app.component.html
      
HTML

<div class="container">
  <h1>Welcome to Kalabar Restaurant and Bukerteria</h1>
  <app-email></app-email>
  <app-order></app-order>
  <app-menu></app-menu>
  <app-payment></app-payment>
  <app-location></app-location>
  <app-delivery></app-delivery>
</div>


menu.component.html

HTML

<div class="menu">
  <h2>Menu</h2>
  <ul>
    <li>Breakfast: Afang Soup with Fufu</li>
    <li>Lunch: Edikaikong Soup with Fufu</li>
    <li>Dinner: Afia Efere with Fufu</li>
  </ul>
</div>


DIAGRAM (Main Component being broken down into Small components(Modules)

Kalabar Restaurant and Bukerteria.
"Welcome to kalabar Restaurant and Bukateria"
  |
  +-- Shell (AppComponent)
       |
       +-- EmailComponent
       +-- OrderComponent
       +-- MenuComponent
       +-- PaymentComponent
       +-- LocationComponent
       +-- DeliveryComponent

blob:https://outlook.office.com/ca9462f8-222b-4d8d-8a76-888782f5be1d
Flow chart: Client( email)—>Web Server—> Web page —> Shell (Component/package) —-> Menu Component —>  Order Component—> Location Component —> Payment Component —> Delivery Component 

blob:https://outlook.office.com/594dcac4-9d9b-4da8-bd64-c7f4101bb5c8

BREAKFAST @ KALABAR RESTAURANT AND BUKERTERIA
​
Welcome Customers —> Morning Menu<— ‘ Afang Soup and Fufu’
BREAKFAST-'Afang Soup With Fufu'> @ KALABAR RESTAURANT AND BUKERTERIA
https://outlook.office.com/ca9462f8-222b-4d8d-8a76-888782f5be1d
LUNCH-->https://outlook.office.com/ca9462f8-222b-4d8d-8a76-888782f5be1d
DINNER-
(Afia Efere<'White Soup'>  @ KALABAR RESTAURANT AND BUKATERIA)https://outlook.office.com/ca9462f8-222b-4d8d-8a76-888782f5be1d
PAYMENT SERVICE https://outlook.office.com/ca9462f8-222b-4d8d-8a76-888782f5be1d

VIDEO OF 'KALABAR RESTAURANT AND BUKATERIA'
4. 
OUTSIDE THE RESTAURANT-https://outlook.office.com/ca9462f8-222b-4d8d-8a76-888782f5be1d



1. Exhaustive Code Breakdown

CODE FOR MAIN(SHELL) COMPONENT
app.module.ts
(This is the main module of the Angular application where all components are declared and imported).

TypeScript

import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent } from './app.component';
import { EmailComponent } from './email/email.component';
import { OrderComponent } from './order/order.component';
import { MenuComponent } from './menu/menu.component';
import { PaymentComponent } from './payment/payment.component';
import { LocationComponent } from './location/location.component';
import { DeliveryComponent } from './delivery/delivery.component';

@NgModule({
  declarations: [
    AppComponent,
    EmailComponent,
    OrderComponent,
    MenuComponent,
    PaymentComponent,
    LocationComponent,
    DeliveryComponent
  ],
  imports: [
    BrowserModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }


CODE FOR MAIN(SHELL)COMPONENT
app.component.html
(This is the main template that includes all the components).

HTML

<div class="container">
  <h1>Welcome to Kalabar Restaurant and Bukerteria</h1>
  <app-email></app-email>
  <app-order></app-order>
  <app-menu></app-menu>
  <app-payment></app-payment>
  <app-location></app-location>
  <app-delivery></app-delivery>
</div>


CODE FOR MENU
Menu.component.html
(This component displays the menu items.)
HTML

<div class="menu">
  <h2>Menu</h2>
  <ul>
    <li>Breakfast: Afang Soup with Fufu</li>
    <li>Lunch: Edikaikong Soup with Fufu</li>
    <li>Dinner: Afia Efere with Fufu</li>
  </ul>
</div>


HTML

<div class="email">
  <h2>Email</h2>
</div>


CODE FOR ORDER
order.component.html
(This component handles order-related functionality).

HTML

<div class="order">
  <h2>Order</h2>
</div>


CODE FOR PAYMENT
payment.component.html
(This component handles payment-related functionality).

HTML

<div class="payment">
  <h2>Payment</h2>
</div>




CODE FOR LOCATION
(This Code - Module/Component displays the restaurant’s location).

HTML

<div class="location">
  <h2>Location</h2>
</div>

 
CODE 
For -Delivery-related functionality.
(This Code Handles Delivery to the Customer-passes information to Delivery Service)

HTML

<div class="delivery">
  <h2>Delivery</h2>
</div>

2. Analysis
The Angular application is structured into several components, each responsible for a specific part of the restaurant’s functionality. This modular approach makes the code easier to manage and maintain. The main AppComponent serves as the shell that includes all other components.

3.Code Testing using Angular's innate Capabilities.
To test the components, we use Angular’s testing utilities along with Jasmine and Karma. 


Testing the MenuComponent.

menu.component.spec.ts
TypeScript

import { ComponentFixture, TestBed } from '@angular/core/testing';
import { MenuComponent } from './menu.component';

('MenuComponent', () => {
  let component: MenuComponent;
  let fixture: ComponentFixture<MenuComponent>;

  beforeEach(async () => {
    await TestBed.configureTestingModule({
      declarations: [ MenuComponent ]
    })
    .compileComponents();
  });

  beforeEach(() => {
    fixture = TestBed.createComponent(MenuComponent);
    component = fixture.componentInstance;
    fixture.detectChanges();
  });

  it('should create', () => {
    expect(component).toBeTruthy();
  });

  it('should display menu items', () => {
    const compiled = fixture.nativeElement;
    expect(compiled.querySelector('h2').textContent).toContain('Menu');
    expect(compiled.querySelector('ul').textContent).toContain('Breakfast: Afang Soup with Fufu');
    expect(compiled.querySelector('ul').textContent).toContain('Lunch: Edikaikong Soup with Fufu');
    expect(compiled.querySelector('ul').textContent).toContain('Dinner: Afia Efere with Fufu');
  });
});



4. Objections, Observations, and Disadvantages
Objections
Complexity: The modular approach can become complex if not managed properly, especially with a large number of components.
Performance: Angular applications can sometimes have performance issues if not optimized correctly.
Observations
Scalability: The modular structure makes it easy to scale the application by adding new components.
Maintainability: Each component is self-contained, making the codebase easier to maintain and debug.
Disadvantages
-Learning Curve: Angular has a steep learning curve for beginners.
-Boilerplate Code: Angular applications often require a lot of boilerplate code, which can be cumbersome, and involves Developers being on the watch , to cancel out such BoilerPlate(Excess)Code generated by the main package(and repeated, across different parts of the project).
-Tailwind:the use of 'Tailwind 'may help mitigate these problems,other stategies are discussed in the 'ADVANTAGES SECTION BELOW '.



ADVANTAGES OF BOILERPLATE CODE.

1. Importance and Implications of Boilerplate Code
Boilerplate Code refers to sections of code that are repeated across different parts of a program or across different projects with little to no modification. It often includes setup and configuration code that is necessary for the application to function but doesn’t contribute to the unique logic of the application.

Importance
Time-Saving: Boilerplate code allows developers to save time by reusing common code structures instead of writing them from scratch for every new project1.
Consistency: It ensures consistency across different projects, which can be particularly important in large teams where multiple developers are working on the same codebase2.
Error Reduction: Using well-tested boilerplate code reduces the likelihood of introducing new errors, as this code has typically been refined and debugged over time1.
Standardization: It helps in maintaining a standard coding practice across projects, making it easier for new developers to understand and contribute to the codebase2.
Implications
Overhead: Boilerplate code can sometimes include more code than necessary, increasing the complexity of the project1.
Lack of Flexibility: Predefined code may not fit every unique application, requiring customization which can be time-consuming1.
Understanding: Relying heavily on boilerplate code may lead to a lack of understanding of the underlying logic, making troubleshooting and updates challenging3.
Herd Mentality: Developers might adopt popular boilerplate solutions without critically evaluating their suitability for their specific project needs3.
2. Mitigating Negative Effects of Boilerplate Code
To mitigate the negative effects of boilerplate code, consider the following strategies:

Customization
Tailor the Boilerplate: Customize the boilerplate code to better fit the specific needs of your project. This ensures that the code is more relevant and efficient for your particular use case3.
Documentation
Comprehensive Documentation: Maintain thorough documentation for the boilerplate code. This helps developers understand the purpose and functionality of the code, making it easier to modify and troubleshoot3.
Modularization
Modular Approach: Break down the boilerplate code into smaller, reusable modules. This makes it easier to include only the necessary parts and avoid unnecessary overhead1.
Regular Review
Periodic Review: Regularly review and update the boilerplate code to ensure it remains relevant and efficient. This helps in identifying and removing outdated or redundant code3.
Education
Training and Education: Ensure that all team members understand the boilerplate code and its purpose. This can be achieved through training sessions and code reviews3.
By implementing these strategies, you can leverage the benefits of boilerplate code while minimizing its drawbacks.

3: Breaking the Myth — Code Boilerplates - DEV Community 1: Understanding Boilerplate: Essential Guide to Boilerplate Code - kinoo 2: Boilerplate Code: Productivity and Consistency in Software Development - IteratorsHQ




SECURITY
There is an adage from Japan :"Business is War"- hence the need to provide adequate security at all levels. As Hackers are constantly on the Prowl- with Malicious intent namely:
1)User Side.
2)Web side.
3)Server side.

1. User Side Security
Input Validation
Sanitize Inputs: Ensure all user inputs are sanitized to prevent injection attacks (e.g., SQL injection, XSS).
Client-Side Validation: Implement client-side validation to provide immediate feedback to users and reduce server load.
Authentication and Authorization
Strong Passwords: Enforce strong password policies and use multi-factor authentication (MFA) where possible.
Session Management: Use secure cookies and manage user sessions properly to prevent session hijacking.
Secure Communication
HTTPS: Ensure all communication between the client and server is encrypted using HTTPS.
2. Web Side Security
Content Security Policy (CSP)
CSP Headers: Implement CSP headers to prevent XSS attacks by controlling the sources from which content can be loaded.
Secure Cookies
HttpOnly and Secure Flags: Set the HttpOnly and Secure flags on cookies to prevent access via JavaScript and ensure they are only sent over HTTPS.
Cross-Site Request Forgery (CSRF) Protection
CSRF Tokens: Use CSRF tokens to protect against CSRF attacks by ensuring that requests are coming from authenticated users.
3. Server Side Security
Input Validation
Server-Side Validation: Validate all inputs on the server side to ensure they meet expected formats and constraints.
Authentication and Authorization
JWT Tokens: Use JSON Web Tokens (JWT) for secure authentication and authorization.
Role-Based Access Control (RBAC): Implement RBAC to ensure users have access only to the resources they need.
Secure Configuration
Environment Variables: Store sensitive information like API keys and database credentials in environment variables.
Regular Updates: Keep all server software and dependencies up to date to protect against known vulnerabilities.
Logging and Monitoring
Audit Logs: Maintain audit logs of user activities and system events to detect and respond to suspicious activities.
Intrusion Detection Systems (IDS): Use IDS to monitor and alert on potential security breaches.
Example Implementation
Angular (User Side)
TypeScript

// Example of input sanitization in Angular
import { DomSanitizer } from '@angular/platform-browser';

constructor(private sanitizer: DomSanitizer) {}

sanitizeInput(input: string) {
  return this.sanitizer.sanitize(SecurityContext.HTML, input);
}

Express.js (Server Side)
JavaScript

const express = require('express');
const helmet = require('helmet');
const csrf = require('csurf');
const cookieParser = require('cookie-parser');

const app = express();

// Use Helmet to set various HTTP headers for security
app.use(helmet());

// Enable CSRF protection
app.use(cookieParser());
app.use(csrf({ cookie: true }));

// Example of JWT authentication middleware
const jwt = require('jsonwebtoken');

function authenticateToken(req, res, next) {
  const token = req.cookies.token;
  if (!token) return res.sendStatus(401);

  jwt.verify(token, process.env.ACCESS_TOKEN_SECRET, (err, user) => {
    if (err) return res.sendStatus(403);
    req.user = user;
    next();
  });
}

app.use(authenticateToken);

// Example route
app.get('/secure-data', (req, res) => {
  res.json({ message: 'This is secure data' });
});

app.listen(3000, () => {
  console.log('Server running on port 3000');
});
CONCLUSION:
Micro Mono-Frontend using ANGULAR FRAMEWORK, developed by Google, to develop our Project 'KALABAR RESTAURANT AND BUKERTERIA'.The term 'Micro Mono-Frontend' is used here , to describe the construction of the project , by a single group(team) of Developers. This has the following :
 -Advantages:
1)Independent Release: by a single group(team) of Developers.
2)Time Saving: the time from conceptualization by the Owner(Individal or Companies),and Development by a single group(team),cut short time to Market,for the product.
3)Increased Speed of Production: by the Owner(Companies).
4)Complexity Reduction :is achieved ,with the focus on single efforts rather than Complex application development.
5)Scalability: is improved , as the focus is on 'few new features addition' by a single team, rather than Multiple Complex addition for the whole application.
6)Decoupling: is archived making the development,testing,and deployment of the product easier.
7)Maintainability:is a big advantage.
8)Technical Debt : is reduced.
-Disadvantages:
1)Error Prone: it is more error prone than having the 'wisdom' of multiple Groups(Teams) of Developers, as novel ideas ,are less likely to be Developed.
2)Rigorous testing :is less likely to take place for the final product.


 Multi-Development Micro Frontend, is rather the work of Multiple Groups of Developers - with the United Goal of producing the same product, with the separate Components(Modules),being handled by Different Teams of Developers. The final product , being finally Harmonized(and brought together), without the User being aware of the joint Cooperation between Developers ,working separately to produce the final product.
This is the Go-To-Method, as it offers the following : 
-Advantages:
1)Innovation: more likely as the' wisdom' and creativity ,from different teams with different perspectives.
2)Enhanced Collaboration: with different teams,resulting in a more cohesive, well integrated final product.
3)Faster Time to Market: as 'many hands' are on the project,thus cutting time.
4)Skill Sets: which are diverse are brought to play, increasing product 'Quality'.
5)Cross Fertilization of Ideas: takes place, as the different teams bring in 'Novel 'ideas on improvement of other teams Module/Components.


