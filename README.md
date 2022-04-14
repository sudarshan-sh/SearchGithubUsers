#  Search Github Users App

[Live Demo](https://do-search-users.netlify.app/)

##  Introduction

*   It is a React application that allows to search github users.

*   Only an authenticated user can do searching of github users.


##  Functional

*   The navigation bar has a welcome user message with his mentioned email along with the logout link.

*   When a visitor searches any github user then other information of that searched user will be displayed such as- 

    *   number of repositories(repos),
    *   number of followers & followings and gists, 
    *   remaining requests to search user in one hour,
    *   name, image, username(if exists), follow button, bio, working company, location and blog of the user(if exists).
    *   most used language(shown by Pie3D),
    *   most starred repos(shown by Column3D), 
    *   most popular language(shown by Doughnut3D),
    *   most forked repos(shown by Bar3D). 

*   The searched user has a list of followers whom also can be followed through their github account.

*   If a searched user doesn't exist a message would be visible above i.e.., There Is No User With That Username and again when existing user is being searched, error goes away.

##  Technical

*   This application is built on **ReactJS** in which visitor has to be logged in to search github users for which a JavaScript based library is used i.e... **Auth0 React SDK** for implementing authentication.

*   Auth0 React SDK has **useAuth0** hook which has been used to access authentication state (isLoading, isAuthenticated and user) and authentication methods (loginWithRedirect and logout).

*   The app also has a library i.e., **FusionCharts** to create interactive charts such as- *Pie3D, Column3D, Doughnut3D and Bar3D*.

*   Other libraries/packages/modules are **axios, react-router-dom, react-icons and styled-components**.

*   Source of data-

    Github User API- https://api.github.com/users/sudarshan-sh
