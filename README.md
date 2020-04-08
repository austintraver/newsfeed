# Newsfeed

## Contributors

Authors | GitHub|
-----------|-------|
|Austin Traver|[@austintraver](github.com/user/austintraver)|
|Claire Powers|[@clairepo](github.com/user/clairepo)|
|Arif Ahmed|[@arifahme](github.com/user/arifahme)|
|Vikash Mody|[@vikasham](github.com/user/vikasham)|

## Deployment

### Environment

This newsfeed application should run fine on any UNIX-like platform, such as Ubuntu 19.04 (Disco Dingo) but has been tested most thoroughly on macOS 10.15 (Catalina).

### Dependencies

#### Homebrew
`$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

#### Java (11.0.2)
`$ brew cask install java`

#### Node (11.12.0)
`$ brew install node`

#### MySQL (8.0.15)
`$ brew install mysql`

#### Yarn (1.15.2)
`$ brew install yarn`

### Installation

First clone this repository on the server that will host the web application.

Once you've entered inside the directory of the cloned repository, type the following commands

```sh
cd ./frontend
yarn install
cd ../backend
yarn install
cd ../
yarn install
yarn global add nodemon
yarn global add create-react-app
```

## Clarification: Java Component

Note that this web application was built in exclusively NodeJS. The java component of this project is part of a different application. The java component is a RESTful server application, *Parsify*, that was once deployed at https://polytime.solutions but has since been taken offline. Parsify runs completely in Java, and is part of our backend. It is a server that, given a request for a particular category of news, finds new articles and returns them to the client.
