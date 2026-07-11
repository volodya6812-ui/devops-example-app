# DevOps example app

This is a simple node application that shows on the main page server on which it is running and report errors to [Rollbar](https://rollbar.com/).

## Usage

```bash
docker run -p 3000:3000 -e SERVER_MESSAGE="Hello, World!" -e ROLLBAR_TOKEN="<your token>" alkselsv/devops-example-app
# open http://0.0.0.0:3000 in browser
```

## Requirements

- Make

## Install

```bash
make setup
```

You may pass environment variable `SERVER_MESSAGE`, and its value shows on the main page.

Edit _.env_ file to set up environment variables.

```env
SERVER_MESSAGE="Hello, World!"
ROLLBAR_TOKEN=<your token>
```

## Start application

```bash
make start
# open http://127.0.0.1:3000 in browser
```
Practice work
