# learning-react

Repositorio para aprender **reactjs** paso a paso

# Paso 00

Se agrega el README.md al repositorio

# Paso 01

Se crea el proyecto usando [create-react-app](https://github.com/facebookincubator/create-react-app)

# Paso 02

Se instalan las dependencias para hacer el linter del código

```bash
npm install --global eslint-config-react-app@0.3.0 eslint@3.8.1 babel-eslint@7.0.0 eslint-plugin-react@6.4.1 eslint-plugin-import@2.0.1 eslint-plugin-jsx-a11y@2.2.3 eslint-plugin-flowtype@2.21.0
```

Se pone en el package.json lo siguiente:

```js
{
  // ...
  "eslintConfig": {
    "extends": "react-app"
  }
}
```

# Paso 03

Se organiza la estrutura del proyecto para tener el punto de entrada **index.js** y llamar
al Componente principal de la aplicación App.js ubicado en el directorio **containers**

# Paso 04

Se instala **redbox-react** para ver un trace log de los errores en un componente de react

```bash
yarn add redbox-react
```

Se agrega  **Hot Module Replacement** (HRM) para cargar solo los módulos que cambian y no toda la aplicación
en desarrollo. Para esto de modifica el archivo **src/index.js**

# Paso 05

Se instalan las dependencias para hacer el linter del código con airbnb

```bash
npm install --global eslint@3.9.1 eslint-plugin-jsx-a11y@^2.2.3 eslint-plugin-import@^2.1.0 eslint-plugin-react@^6.6.0 eslint-config-airbnb@13.0.0
```

Se pone en el package.json lo siguiente:

```js
{
  // ...
  "eslintConfig": {
    "extends": "eslint-config-airbnb",
    "env": {
      "browser": true,
      "node": true
    },
    "parser": "babel-eslint",
    "rules": {
      "semi": [2, "never"],
      "react/no-multi-comp": 0,
      "import/default": 0,
      "import/no-duplicates": 0,
      "import/named": 0,
      "import/namespace": 0,
      "import/no-unresolved": 0,
      "import/no-named-as-default": 2,
      "comma-dangle": 0,  // not sure why airbnb turned this on. gross!
      "indent": [2, 2, {"SwitchCase": 1}],
      "react/jsx-boolean-value": 0,
      "react/jsx-first-prop-new-line": 0,
      "react/jsx-filename-extension": [1, { "extensions": [".js", ".jsx"] }],
      "no-console": 0,
      "no-alert": 0
    } 
  }
}
```

