# learn-tailwind-css

## What is Taiwind CSS?

- CSS framework made up of utility classes.
- Much lower-level than bootstrap, Materialize etc..
- In tailwind css there is no pre-builded components there are some classes for achieving some special styles.
- It provides more flexibility.

## How to use Tailwind CSS?

### 1st Method

- Install tailwind CSS Using NPM(Node Package Manager).
- You will need to install node.js in your computer(you can download node from - nodejs.org/en).
- node -v => For checking node version.
- npm init -y => Helps to create a new package.json using npm.
- npm install tailwindcss => for install tailwind css.

### 2nd Method

- Open to the folder and terminal
- Run 'npm init -y'
- Run 'npm install tailwindcss' if you need autoprefixer then use the command 'npm install tailwind autoprefixer'.
- RUn 'npm install postcss-cli'
- For create cofiguration files run the command 'npx tailwindcss init -p'
  - This also create the postcss config file along with tailwind.configjs.
- Create folders named 'src and public'
- In public folder create files named 'index.html and styles.css'
- In src folder create file named 'styles.css'
- Fill styles.css file in src folder using this codes :-

  ```
    @tailwind base;
    @tailwind components;
    @tailwind utilities;

  ```

- Change script object with

  ```
  "build":'postcss .src/styles.css -o ./public/styles.css'
  ```

- Then run 'npm run build' command in terminal.

- if you get an error like ' TypeError :Object.entries(...).flatMap is not a function'
  then one of the main reason of this error caused is old node version.
  to install latest verison of node run 'nvm install node'.

## How tailwind works?

- style.css(source file) => Tailwind => styles.css => index.html
