## Work / Project Examples

1. Lethbridge Food Guide: Please see the link here [Lethbridge Food Guide](https://github.com/leechingching/leth-food-master) to explore the web app.

   Role: Web Developer and Designer

   Idea: This is version 2.0 of my Food Guide app. Living in Lethbridge can be difficult for young people and new students who are looking for places to hangout at with friends, or restaurants to dine at. I'd like to make Lethbridge more interesting by providing information about popular places to eat at to the residents here. Instead of providing specific data to users, this app will provide a random result.

After my internship and part-time job, this is my first individual web project that I worked on while learning React. I created custom components to call and render the Zomato API. For this project, my main focus is the functionality and React, therefore, I did not spend as much time with the CSS. The UI design is very similar to my first project, but it is more responsive and dynamic.

---

2. Textbooks of Terrors: Please see the link here [Textbooks of Terrors](http://jekyll.chingchinglee.com/projects/textbooks_of_terrors/) to explore this Education App.

   Role: UI Designer

   Idea:
   The idea behind the app was generated largely at Coalbanks elementary school. We met with a small group of grade 5 students and spoke with them about the types of apps they used, and what they like about them. We also spoke to them about what they were learning about in school and what they would like to see in an educational app. The grade 5s were very vocal about their experiences with apps and what they hoped to see in an app. From that discussion, we came up with our idea.

   The App will take place as a story/adventure game wherein the Coalbanks school mascot Colby (above) will approach the player and ask them to come to Coalbanks school, where the teachers of the school have been taken/imprisoned by their Alter Egos. The player has to save the teachers by exploring the school, finding the teacher’s classrooms and solving various puzzles or questions posed by the Alter Egos of the school. The activities will be linked to the GLOs and SLOs of the Grade 4/5 alberta curriculum. The game is over when all the teachers have been freed.

   Our app is specifically designed for Coalbanks elementary school and their students. Therefore, we will simulate the real environment of the school. The following elements will be included:

   - Photos of the environment of Coalbanks (such as Hallway, classrooms)
   - Colby as the game’s instructor/helper
   - Cartoon drawing of their teachers
   - Sound effects and animation
   - Missions and Tasks: to solve Academic questions

   Both audience groups will gain benefits from this app. On the one hand, Coalbanks elementary school can promote their school in a more interesting and modern way. On the other hand, their students can learn useful academic knowledge as well as get additional information about their school.

   My main role is to design the path of the game, and how/where to put the UI elements in order to lead a logical store flow, and make sure students can understand the functionality of the app.

## Inspiration

1. [srcset and sizes attributes](https://www.youtube.com/watch?v=2QYpkrX2N48)

   This youtube video inspires me to rethink the definition of "responsive design" and how to create a modern responsive design. Before I watched this youtube video, I was creating the web for the machine because I thought responsive design simply mean resize the element, and make it fit on every device. Human and machine are two kinds of audiences, machine only needs the code and training data to understand the functionality of the app, but human needs logical website structure and graphic design to understand the purpose and data of the web app. Therefore, responsive design should respond to logical functionality as well.

   This video shows the method to load in different versions of the same image based on the size of the viewport or the pixel density of the user's device. If we only set `{img: 100%;}`, it will be responsive but it may not make sense to human. When users start narrowing the screen device, the browser is going to increase the screen height. On the mobile device, it may be very difficult to see the small detail on the image. Also, it is not ideal if we use a larger image to handle the responsive design because it takes time to download for mobile users. Instead of only setting `{img: 100%}`, it does not hurt if we use:

   ```
   <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/308367/cat-500.jpg"
        srcset="https://s3-us-west-2.amazonaws.com/s.cdpn.io/308367/cat-500.jpg 500w,
                https://s3-us-west-2.amazonaws.com/s.cdpn.io/308367/cat-1000.jpg 1000w"
        sizes="(min-width: 600px) 50vw, 100vw"
        alt="">
   ```

   to display different images based on based on the size of the viewport. It provides a better UI and UX, and also fix the large image donwload problem.

   HTML, CSS and JavaScript is a part of the responsive design. Getting a better understanding of how responsive design function is the requirement to coding an user-friendly site.

---

2. [CSS Grid: Floor Plan](https://codepen.io/oliviale/pen/moLrBq)

   This Codepen inspires me to use CSS Grid in a more interesting way and experiment with the limits of this method. Now I think about web layout in new ways. This Codepen uses CSS Grid and CSS transforms property to create the floor plan, it does not include any JavaScript or additional library.

   ```
   .bathroom-2 {
      grid-column: 5 / span 2;
      @include border;
      border-width: 0 0 4px 4px;
      
         .rug {
            width: 45px;
            height: 25px;
            top: 45%;
            left: 25px;
            transform: rotate(-40deg);
            z-index: 20;
         }
         
         .door-hor {
            bottom: -4px;
            left: 40px;
            transform: rotate(180deg);
         }
         
         .window-hor {
            left: 30px;
         }
         .toilet {
            left: auto;
            right: 8px;
         }
         .vanity {
            bottom: auto;
            top: -2px;
            width: 50px;
         }
   }
   ```

   With CSS Grid, we can do a lot of interesting web graphic without adding an image which will low down the page speed. It also shows us another possibility that developer can use CSS Grid to align HTML elements to create web animation without using SVG. Although it may not be the best practice, it shows another possibility to developer to experiment this method. Developer now have more flexability to create a better responsive design using CSS Grid, as this inspiration shows:

   ```

   .kitchen {
      grid-row: 1 / span 3;
      grid-column: 3 / span 2;
      
      .island {
         position: absolute;
         width: 100px;
         height: 45px;
         @include utility-border;
         top: 100px;
         left: 50px;
         
            &:before,
            &:after,
            .chair {
               @include utility-border;
               content: "";
               position: absolute;
               width: 25px;
               height: 25px;
               bottom: -35px;
               border-radius: 50%;
               left: 5px;
               background: \$color-shade;
         }
   }

   ```

   We are able to use position within the grid item to create our graphic. It makes our CSS code look much more clean that we can maintain and modifiy easier later.

   This example shows that CSS Grid removes many limitations that existed in the front end world. And it eases the border between developer and designer since it provides a better for them to communicate and work together. Designer can design fancier and unique web layout and developer can create the design without worring the 12-column grids!

## Focus

If I am lucky enough to be select to be one of the team member this summer, I'd love to spend my time learning 1. [PWA](https://developers.google.com/web/progressive-web-apps/) and 2. [React](https://reactjs.org/), and also mastering my favourite langauge CSS, specifically 3. [CSS GRID](https://learn.freecodecamp.org/responsive-web-design/css-grid/). I will spend most of my time learning React since the high demand, and I prefer to add CSS Grid to the web project. I will spend my own time to learn PWA, and communciate with other developers to know their opinions and experience on PWA.

1. PWA

Since mobile device has dominated the majority of the web market. Most users still spend most of their time playing native apps instead of searching web apps. Therefore, users are not engaged much. With PWA, users can download the app web to their mobile device with one-click, and they can use it whenever they want and take all the main information and function from the web app. I believe it is the future trend of the web development market, and Google has highly promoted this PWA concept. It is always a good idea to learn the new trend and skills as soon as possible in order to launch the PWA when the market is ready.

2. React

ReacT is one of the popular frameworks, and it is getting more and more built-in functions. The React 16.8 add "Hooks" which makes our lives easier and the app better. React sorta become an industry standard and the requirement of front end developer since a lot of international companies and brands are using React to rewrite their sites. And also, JavaScript and React are improving at the same time, it is interesting to master your javaScript and learning new React features at the same time.

3. CSS GRID

CSS is always my favorite markup language as it enchants your sites and makes your sites look different. CSS layout is never an easy job for developers, and mobile device increases the difficulty of CSS layout. Before the CSS group created CSS Grid, we used Float, position, and Flexbox to align our items, and we need to write many fallback codes to support the old browser. It is a pain in the ass to me. Although we can use Bootstrap to solve most of the layout problems, it makes our site boring.

CSS Grid provides the possibility for us to create a responsive and unique web layout which makes our web apps look awesome and different! With CSS Grid, we can make an awesome layout without adding JavaScript. Also, we can maintain and understand our code easier. As I said before, mobile device is taking over the web market. Therefore, most of the web apps are going to show on a specific resolution and width. Therefore, using CSS Grid can provide a wonderful UI and UX for this environment.

Nowadays, CSS Grid has better browser support and being one of the popular layout methods. I am so excited to learn the CSS Grid 2.0 (subgrid) and use CSS Grid in a more interesting way. I look forward to building CSS Grid layouts on the web which will support most modern browsers.

## CodeChallenge

Please see [CodeSandBox](https://codesandbox.io/s/3v13wv4v7p)
