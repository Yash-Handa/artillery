# artillery

A fully loaded CRA (create react app) template

## USAGE

```cmd
npx create-react-app my-app --template artillery
```

## Features (utilities)

1. LocalTunnel support
2. jsconfig configuration
3. editorconfig support
4. prettier support
5. eslint support
6. browserlist support
7. .env support
8. css normalization
9. source map explorer support

**NOTE**: Remove eslintConfig and browserslist from package.json

## File Structure

Artillery is a CRA (create-react-app) template which modify some files and add some to the CRA module.
Below are all the files which have been modified / added as per the artillery template.

```
project
│
└─custom_scripts
│   └─localTunnel.js
│
└─src
│   └─index.css
│   └─index.js
│
└─.browserslistrc
└─.editorconfig
└─.env
└─.eslintignore
└─.eslintrc.json
└─.prettierrc
└─.jsconfig.json
└─package.json
```

### LocalTunnel support

The project is configured to integrate with localtunnel out of the box. Localtunnel allows the developer's work environment to be exposed to a public https domain which can be used by anyone with that url to access the project in it's development phase. The localTunnel can be fine tuned(customized) in `custom_scripts/localTunnel.js` file.

**usage:**

```cmd
npm run lt
```

### jsconfig configuration

`jsconfig.json` is a json file which helps better integration with vs-code. Note that this file is only useful for vs-code. Read here for configuration options in jsconfig.

### editorconfig support

`.editorconfig` is used for setting up defaults for all the browsers. Read here for configuration options. It is recommended to use the editor specific extensions for better integration.

### prettier support

Prettier is one of the most famous code formatter present and works very well with most of the code editors. Prettier is configured as a plugin of eslint and works seamlessly with eslint. `.prettierrc` file contains the configurational details of prettier. Read here for prettier configurational options.

Though prettier being an eslint plugin runs every time eslint runs but if you want to use it separately use the following command:

```cmd
npm run fix-formate
```

It is recommended to use the editor specific extensions for better integration.

### eslint support

Though CRA comes with eslint support in-build but Artillery template extends it further with prettier plugin and eslintignore file. Use `.eslintrc.json` for adding customized eslint rules. Use `.eslintignore` for excluding files from eslint. CRA will run eslint automatically but it is preferred to use a editor specific extensions for better integration.
