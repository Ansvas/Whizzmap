## Hasura Hub - Read Me

### Introduction

WhizzMap is a simple Mapbox based Quick-start Hasura project which consists of 
- a React JS based Web app
- a ReactNative based mobile app 
- a Python Flask back-end API

### Contributors:

    • React JS – Web app :          Sathya Bhupal Reddy (https://github.com/sathya9897)
    • React Native – Mobile App :   Padmavathy Balasundararaj (https://github.com/padmasaravan)
    • Backend – Python -Flask :     Vinitha (https://github.com/vinitha-shree)
                                    Anshul Sharma (anshul60198@gmail.com)
                               
### What does this come with?

Custom service that integrates with **Mapbox Maps SDK** and has **Hasura.io** as _BaaS_

    • Allows the user to enter the source, destination and the mode of transportation ( Driving / Cycling / Walking )
    • Shows the shortest route to the destination from the source/starting point
    • Displays the Time taken for travel & the total Distance between the two places
    • User can also view the Directions to travel from source to destination
    
### Pre-requisites
- Mapbox API token - Find instructions to get one [here](https://www.mapbox.com/help/how-access-tokens-work/)
- Hasura CLI - instructions to download latest version from [here](https://docs.hasura.io/0.15/manual/install-hasura-cli.html)
- Hasura Hub Account
- Gitbash (recommanded)
    
### Getting the Hasura project
```bash
    $ hasura quickstart sathya/whizzmap
  $ cd whizzmap
    
  # Deploy
  $ git add . && git commit -m "Deployment commit"
  $ git push hasura master
```
After the git push completes:
```bash
    $ hasura microservice list
```
- The ```hasura quickstart``` command clones the project repository to your local computer, and also creates a free Hasura cluster,   where the project will be hosted for free.
 
- A git remote (called ```hasura```) is created and initialized with your project directory.  

- Get the name of your cluster by running the command ```hasura cluster status```

- Open the flask app url in browser **https://app.cluster-name.hasura-app.io/** so that python flask microservice is started. If you get a message stating that the cluster is waking, wait for a minute or two and try accessing it again. Once the page displays **WhizzMap**, everything is working as expected - the microservice is started and ready to accept your API endpoint requests.
- To check out the ReactJS Web version in action, open the  url **https://ui.cluster-name.hasura-app.io/** in the browser
- Demo video of the React Native app is in this [link](https://youtu.be/au0cL47_inU)

### Local Development

Check out the ReadMe files of the respective folders.
- **ReactJS** ( Web App) - whizzmap/microservices/ui/app/
- **Python-Flask** (Python Flask) - whizzmap/microservices/app/
- **React Native** (Mobile App) - whizzmap/react-native/README-ReactNative.md

    

