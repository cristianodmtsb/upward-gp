# USAGE

```
$ yarn add @cristianodmtsb/upward-gp
```

Then open the `webpack.config.js` file, find the usage of `configureWebpack` method and add the following block inside the `special` node:

```
'upward-gp': {
    cssModules: false,
    esModules: false,
    graphqlQueries: true,
    rootComponents: false,
    upward: true
}
```

It will be like this:

```
special: {
    'react-feather': {
        esModules: true
    },
    '@magento/peregrine': {
        esModules: true,
        cssModules: true
    },
    '@magento/venia-ui': {
        cssModules: true,
        esModules: true,
        graphqlQueries: true,
        rootComponents: true,
        upward: true
    },
    'upward-gp': {
        cssModules: false,
        esModules: false,
        graphqlQueries: true,
        rootComponents: false,
        upward: true
    }
},
```
