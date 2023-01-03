# Theory:

* What is Emmet?

    Plugin for various editors which enables the web-developers, to generate code structure though simple shortcuts / abbreviations.
    e.g.: 
    ```
    <!-- 
    Refer [assignment-01.html](assignment-01.html)
    Typing: 
    #main>#header+#body+#footer
    Quickly creates the following HTML structure:
    -->
    <div id="main">
        <div id="header"></div>
        <div id="body"></div>
        <div id="footer"></div>
    </div>
    ```

* Difference between a Library and Framework?

    Library is program which solves specific problem like, rendering a chart, providing predefined reuseable-css classes, for displaying font-icons, modifying date time object, displaying customizable calender widgets, etc...
    e.g.: momentjs, bootstrap, chart-js, calendar.js, font-awesome, React, etc...

    Framework is a program that may be include set of libraries, which is used to build an entirely new application by following the syntax / rules & best practices suggested by the framework docs.
    e.g.: Angular, Vue.js, Node.js, NextJS, 

* What is CDN? Why do we use it?

    CDN is short form for Content Delivery Network. As the name suggests, it is used for delivery content to other websites / web-apps from different origin. This is commonly used, in order to:
    - increase the delivery speed of commonly used libraries / frameworks / images / media files
    - reduce the load on the server where the main application is being hosted and maybe used by plethora of users.

    This is achieved by creating a group of servers distributed across the globe which effectively brings the requested content from the location which is more closer to the users.

* Why is React known as React?

    The idea of react project is to create multiple components which communicates with each other to form a single usable application, is some thing similar to how physical objects work in an atomic level. With that similar idea in mind of the root developers, the term react was coined denoting the reaction between atoms / components.

    As pointed out by Dan Abromav [in this video](https://www.youtube.com/watch?v=dpw9EHDh2bM&t=3455s).

* What is crossorigin in script tag?

    `crossorigin` attribute enables CORS settings when a CDN link is being passed to the `src` attribute of the script tags. Since the CDN links points to different domain, it makes sense to enable CORS header while making a request to a CDN.

* What is difference between React and ReactDOM?

    React is a library used for creating html elements & components. Whereas ReactDOM is used for rendering the elements created by react library to the DOM.

*  What is difference between react.development.js and react.production.js files via CDN?

    `.development.js` is the original code file containing the plain js code. `.production.js` is a minified and optimized for production use. So the later is definitely faster to load in the production deployment.

* What is async and defer?

    `async` and `defer` are the attributes added to a script tag to improve the HTML content loading. 

    The default behavior while loading html page containing script tag:

        - The page loading gets halted till the time the script is downloaded & processed by the browser
    
    When `async` attribute is added to the script tag:

        - The page loading continues till the time the script is downloaded & then gets halted till the script is processed by the browser

    When `defer` attribute is added to the script tag:
    
        - The page loading is completed without any halt and then the script is downloaded & processed by the browser