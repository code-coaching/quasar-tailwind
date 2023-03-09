# Quasar Tailwind (quasar-tailwind)

A Quasar template combined with TailwindCSS, provided by [Code Coaching](https://code-coaching.dev).

## Start from this template

### Manual

Download the .zip file and extract it in your project folder.

### Command line

This commando can be used in an existing git repository. It will download the latest version of this template and extract it in a folder named `quasar-tailwind-main`.

```sh
curl -L https://github.com/code-coaching/quasar-tailwind/archive/refs/heads/main.zip | tar -xz
```

In case you want it to be in the root of your project, you can use these commandos:

```sh
mv quasar-tailwind-main/* ./
```

```sh
rm -rf quasar-tailwind-main
```

## Install the dependencies

```bash
yarn
# or
npm install
```

### Start the app in development mode (hot-code reloading, error reporting, etc.)

```bash
quasar dev
```

### Lint the files

```bash
yarn lint
# or
npm run lint
```

### Format the files

This will also sort the classes to have a consistent order.

```bash
yarn format
# or
npm run format
```

### Build the app for production

```bash
quasar build
```

### Customize the configuration

See [Configuring quasar.config.js](https://v2.quasar.dev/quasar-cli-vite/quasar-config-js).
