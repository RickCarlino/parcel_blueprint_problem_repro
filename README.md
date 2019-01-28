# Possible Breakage in Parcel?

Pasting here so others can find this off of Google:

```
🚨  ___/index.scss:1:1: Cannot resolve dependency '~@blueprintjs/core/lib/css/blueprint.css' at '___/~@blueprintjs/core/lib/css/blueprint.css'
    at Resolver.resolve (parcel-bundler/src/Resolver.js:70:17)
    at <anonymous>
```

# Background Info

```
$ parcel --version
1.11.0
```

```
$ npm show @blueprintjs/core

@blueprintjs/core@3.12.0 ....

```

# Setup

```
git clone ____
cd ____
npm install
```

# Reproduce

```
parcel build ./index.scss
```

# Other Information

The example found in `index.scss` is identical to code provided in the [Blueprintjs documentation](https://blueprintjs.com/docs/#blueprint/getting-started.installing-blueprint) and has been working OK in a [project that uses webpack in production](https://github.com/FarmBot/Farmbot-Web-App/blob/staging/webpack/css/_index.scss#L2).
