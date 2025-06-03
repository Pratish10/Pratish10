<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

<!--h1 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h1 style="display: inline-block">Hi 👋, I'm Pratish Ninawe</h1></summary>
  </ul>
</div>

## UML Class Diagram

```mermaid
classDiagram
    %% --------- Models ---------
    class Users {
        - id: String
        - primaryEmail: String
        - secondaryEmail: String?
        - contact: String?
        - fullName: String?
        - userName: String?
        - magicToken: String?
        - refreshToken: String?
        - isCompleted: Boolean
        - location: String?
        - bio: String?
        - twitter: String?
        - instagram: String?
        - website: String?
        - profileIcon: Int
        - eventParticipationEnabled: Boolean
        - isDeleted: Boolean
        - createdAt: DateTime
        - updatedAt: DateTime
    }

    class Update {
        - id: String
        - userId: String
        - eventId: String
        - content: String
        - isNotification: Boolean
        - scheduledNotificationTime: DateTime?
        - isDeleted: Boolean
        - createdAt: DateTime
        - updatedAt: DateTime
    }

    class Event {
        - id: String
        - creatorId: String
        - name: String
        - slug: String
        - category: String?
        - startTime: DateTime
        - endTime: DateTime
        - eventDate: DateTime
        - description: String?
        - eventImageUrl: String?
        - venueType: VenueType
        - venueAddress: String?
        - venueUrl: String?
        - hostPermissionRequired: Boolean
        - capacity: Int?
        - isActive: Boolean
        - isDeleted: Boolean
        - createdAt: DateTime
        - updatedAt: DateTime
    }

    class Attendee {
        - id: String
        - userId: String
        - eventId: String
        - registrationTime: DateTime
        - hasAttended: Boolean
        - checkInTime: DateTime?
        - feedback: String?
        - qrToken: String
        - status: Status
        - allowedStatus: Boolean
        - isDeleted: Boolean
        - createdAt: DateTime
        - updatedAt: DateTime
    }

    class Cohost {
        - id: String
        - userId: String
        - eventId: String
        - role: Role
        - isDeleted: Boolean
        - createdAt: DateTime
        - updatedAt: DateTime
    }

    %% --------- Enums ---------
    class Status {
        <<enum>>
        GOING
        NOT_GOING
        WAITING
        PENDING
        INVITED
        CANCELLED
    }

    class Role {
        <<enum>>
        CREATOR
        MANAGER
        READ_ONLY
        CELEBRITY
    }

    class VenueType {
        <<enum>>
        PHYSICAL
        VIRTUAL
        LATER
    }

    %% --------- Associations ---------
    Users "1" <-- "*" Update    : user  
    Event "1" <-- "*" Update    : event  
    Users "1" <-- "*" Event     : creator  
    Event "1" <-- "*" Attendee  : attendees  
    Users "1" <-- "*" Attendee  : user  
    Event "1" <-- "*" Cohost    : cohosts  
    Users "1" <-- "*" Cohost    : user  
```

<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">A Passionate Developer</h2></summary>
  </ul>
</div>

<!--- description -->
<div id="user-content-toc">
  <ul align="center">
    <summary><p style="display: inline-block">Hi, Welcome. I’m Pratish Ninawe, and I am passionate about coding and designing new things. I have completed my bachelor's in IT with background in Full Stack Web Engineer and I am a self-taught programmer. I am a Frontend Developer with 2 years of experience building scalable, user-centric web applications using JavaScript, React, and modern frameworks. Proficient in delivering robust solutions, collaborating in agile teams, and contributing to both frontend and backend development.</p></summary>
  </ul>
</div>

<!--Intro start-->
- 👯 I’m looking to collaborate on **on any technologies or framework**

- ☁️ I've keen interest in Web development.

- 💬 Ask me about **Reactjs, Nodejs, AWS, MongoDB, Devops**

- 📫 How to reach me **pratish.1006@gmail.com**

- 🏠 Have a look at my [Resume](https://docs.google.com/document/d/11dSCxeD7p5ydPSoxJ_0Kui2vFl-oW4RklmYUXuL9DpA/edit?usp=sharing).
<!--Intro end-->

<!--- stats & Trophy (start) -->
<p align="center">
  <!--- stats (start) -->
<table align="center">
<tr border="none">
<td width="50%" align="center">
  
  <img align="center" src="https://github-readme-stats.vercel.app/api?username=pratish10&theme=dark&show_icons=true&locale=en" alt="pratish10" />
  <br></br>
  <img  title="🔥 Get streak stats for your profile at git.io/streak-stats" alt="Mark streak" src="https://github-readme-streak-stats.herokuapp.com/?user=pratish10&theme=dark&hide_border=false" /> 
</td>

<td width="50%" align="center">

  <img  align="center"  src="https://github-readme-stats.anuraghazra1.vercel.app/api/top-langs/?username=pratish10&theme=dark&hide_border=false&no-bg=true&no-frame=true&langs_count=10"/>
  
  </td>
</tr>
</table>
<!--- stats (end) -->

<!--- trophy (start) -->
<div align=center>
  <a href="https://github.com/ryo-ma/github-profile-trophy" title="Go to Source">
      <img src="https://komarev.com/ghpvc/?username=pratish10&label=Profile%20views&color=0e75b6&style=flat" alt="pratish10" />
    </a>
</div>
<!--- trophy (end) -->

</p>        
<!--- stats & Trophy (end) -->

<!--h1 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Technologies That I Know👨🏻‍💻</h2></summary>
  </ul>
</div>
<!--tech stack icons-->
<p align="center">
  <p align="left"> <a href="https://aws.amazon.com/amplify/" target="_blank" rel="noreferrer"> <img src="https://docs.amplify.aws/assets/logo-dark.svg" alt="amplify" width="40" height="40"/> </a> <a href="https://aws.amazon.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/> </a> <a href="https://www.gnu.org/software/bash/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/gnu_bash/gnu_bash-icon.svg" alt="bash" width="40" height="40"/> </a> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a> <a href="https://www.chartjs.org" target="_blank" rel="noreferrer"> <img src="https://www.chartjs.org/media/logo-title.svg" alt="chartjs" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://expressjs.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original-wordmark.svg" alt="express" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://graphql.org" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/graphql/graphql-icon.svg" alt="graphql" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.jenkins.io" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/jenkins/jenkins-icon.svg" alt="jenkins" width="40" height="40"/> </a> <a href="https://kubernetes.io" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/kubernetes/kubernetes-icon.svg" alt="kubernetes" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/> </a> <a href="https://www.nginx.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nginx/nginx-original.svg" alt="nginx" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a> <a href="https://www.postgresql.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="postgresql" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> <a href="https://redux.js.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redux/redux-original.svg" alt="redux" width="40" height="40"/> </a> <a href="https://www.typescriptlang.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="40" height="40"/> </a> <a href="https://www.vagrantup.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/vagrantup/vagrantup-icon.svg" alt="vagrant" width="40" height="40"/> </a> <a href="https://vuejs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vuejs/vuejs-original-wordmark.svg" alt="vuejs" width="40" height="40"/> </a> </p>
</p>

<!-- Connect with me -->
<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Connect With Me🤝</h2></summary>
  </ul>
</div>

<!--icons and links-->
<p align="center">
<a href="https://www.linkedin.com/in/pratish-ninawe-6199b2220/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="https://www.linkedin.com/in/pratish-ninawe-6199b2220/" height="30" width="40" /></a>
<a href="https://www.facebook.com/pratish.ninawe/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="https://www.facebook.com/pratish.ninawe/" height="30" width="40" /></a>
<a href="https://www.instagram.com/pratish.10/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="https://www.instagram.com/pratish.10/" height="30" width="40" /></a>
<a href="https://leetcode.com/pratish10/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/leet-code.svg" alt="https://leetcode.com/pratish10/" height="30" width="40" /></a>
  
</p>

<!--profile visit count-->
<div align="center">
  
<p> <img src="https://komarev.com/ghpvc/?username=pratish10&label=Profile%20views&color=0e75b6&style=flat" alt="pratish10" /> </p>
  
</div>

<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
