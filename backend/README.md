# Notes

[Original Document Link](https://dev.to/andrewbaisden/how-to-use-eslint-and-prettier-for-code-analysis-and-formatting-1b4g)

## Project Initialization

```bash
    mkdir backend
    cd backend
    npm init -y
    npm install eslint eslint-config-prettier eslint-plugin-prettier --save-dev
```

```console
bulent@Bulents-MacBook-Pro-M1 backend % npm init @eslint/config
Need to install the following packages:
  @eslint/create-config
Ok to proceed? (y) y
✔ How would you like to use ESLint? · problems
✔ What type of modules does your project use? · commonjs
✔ Which framework does your project use? · react
✔ Does your project use TypeScript? · No / Yes
✔ Where does your code run? · browser
✔ What format do you want your config file to be in? · JSON
The config that you've selected requires the following dependencies:

eslint-plugin-react@latest @typescript-eslint/eslint-plugin@latest @typescript-eslint/parser@latest
✔ Would you like to install them now? · No / Yes
✔ Which package manager do you want to use? · npm
Installing eslint-plugin-react@latest, @typescript-eslint/eslint-plugin@latest, @typescript-eslint/parser@latest

added 94 packages, and audited 182 packages in 8s

66 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
Successfully created .eslintrc.json file in /Users/bulent/git-repos/eslint-and-prettier-usage/backend

bulent@Bulents-MacBook-Pro-M1 backend % 
```

Now run the commands in the code block below to create files for prettier.

```bash
    npm install --save-dev --save-exact prettier
    echo {}> .prettierrc.json
```

[Current .eslintrc.json file](.eslintrc.json)

[Current .prettierrc.json file](.prettierrc.json)

```shell
    touch .prettierignore .eslintignore
```

Add these lines to .prettierignore and .eslintignore files:

```shell
    .DS_Store
    node_modules
    package.lock.json
    build
```
