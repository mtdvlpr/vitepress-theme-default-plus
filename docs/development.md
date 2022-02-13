# Development

## Requirements

([Lando](https://lando.dev/)) **OR** ([Node 14+](https://nodejs.org/en/download/) and [Yarn](https://classic.yarnpkg.com/lang/en/docs/install))

:::tip Yarn is optional
`yarn` is technically optional but is preferred and is assumed in the docs below. That said you can probably use `npm` as a drop in replacement for `yarn` below and end up in the same place.
:::

:::: code-group
::: code-group-item LANDO

```bash:no-line-numbers
# clone repo
git clone https://github.com/lando/vuepress-theme-default-plus.git &&
  \ cd vuepress-theme-default-plus

# start up app
lando start

# launch dev server
lando dev
```

:::
::: code-group-item YARN

```bash:no-line-numbers
# clone repo
git clone https://github.com/lando/vuepress-theme-default-plus.git &&
  \ cd vuepress-theme-default-plus

# install deps
yarn

# launch dev server
yarn dev

# launch dev server in debug mode
DEBUG="@lando/*" yarn dev
```

:::
::::

## Testing

:::: code-group
::: code-group-item LANDO

```bash:no-line-numbers
# lint the code
lando yarn test
```

:::
::: code-group-item YARN

```bash:no-line-numbers
# lint the code
yarn test
```

:::
::::

## Releasing

:::: code-group
::: code-group-item LANDO

```bash:no-line-numbers
# build the site
lando yarn build

# deploy the site
lando yarn release
```

:::
::: code-group-item YARN

```bash:no-line-numbers
# build the site
yarn build

# deploy the site
yarn release
```

:::
::::