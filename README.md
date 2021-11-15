# Kick start React project in type-script from scractch

#### Initialize **_git_** in your project

Run the following command to create **_.git_** folder in your project. Which going to maintain all your project history and commits

```sh
git init
```

#### Create a new File name as **_.gitignore_** - in project level

Where you will declare what are the folders and files to be excluded while you push code to **_git_**

#### Create a folder named as **_src_** - in project level

Where you going to make your hands dirty

#### Create a folder named as **_build_** - in project level

There you find **_output_** for your work.

#### Run following command to create **_package.json_** - in project level

which will going to contain all the **project informations**, **dependencies**, **dev-dependencies**, **scrips**, **etc.,** for our project

```sh
yarn init --y
```

#### Create a **_index.html_** file - in project level

File which going to render our **SPA** app in your Browser.

#### Let's Add our first package or **_dependency_** for our project

```sh
yarn add react react-dom
```

- **react** - is used to access react features
- **react-dom** - is used to render our .js || .jsx || .tsx file in browser

### Add Entry point to our Project

#### Create **_index.js** file - in **src** folder

Add the following piece of coding. Which will be the entry point of source folder so this will be rendered in browser

```sh
import ReactDOM from 'react-dom'
import App from './App'

ReactDOM.render(<App />, document.getElementById('root'))
```

#### Create **_App.js** file - in **src** folder

Add the piece html coding to be rendered

```sh
const App = () => {
  return
      <h1>
        Hello This is sample App
      </h1>
}

export default App
```
#### Write **_script_** in **package.json** file

- To run in browser
- To create build
- Other scrips

Write the piece of coding as follows

```sh
  "scripts": {
    "start": "webpack serve --config webpack/webpack.config.js --open",
    "build": "webpack --config webpack/webpack.config.js --open",
    "test": "echo \"Error: no test specified\" && exit 1",
  },
```
# NOTE

```sh
1. SPA => Single Page Application
2. MPA => Multiple Page Application
```
