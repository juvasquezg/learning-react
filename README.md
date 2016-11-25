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
