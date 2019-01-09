# ncc and pkg tools demo

A simple demo of

* compiling a NodeJS project into single file using [ncc](https://zeit.co/blog/ncc)
* creating a standalone executable using [pkg](https://www.npmjs.com/package/pkg)

The target application is created using [Nest](https://nestjs.com/) TypeScript starter template.

## Installation

Install `ncc` and `pkg` globally.

```bash
$ yarn global add @zeit/ncc
$ yarn global add pkg
```

Clone and set up this repository.
```bash
$ git clone https://github.com/shikshan/ncc-pkg-demo.git
$ cd ncc-pkg-demo
$ yarn install
```

## Running the app

```bash
# development
$ yarn start

# watch mode
$ yarn start:dev

# production mode
yarn start:prod

# bundle the application into a single file and a distributable.
# Check distro script in package.json for details.
yarn distro

# run the single file
yarn start:ncc

# run the standalone executable. It starts executable for mac, change as per your OS.
yarn start:pkg
```
