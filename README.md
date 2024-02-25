# learn-cicd-starter (Notely)

![code coverage badge](https://github.com/sharifmu/learn-cicd-starter/actions/workflows/ci.yml/badge.svg)

This repo contains the starter code for the "Notely" application for the "Learn CICD" course on [Boot.dev](https://boot.dev).


## Local Development

Make sure you're on Go version 1.20+.

Create a `.env` file in the root of the project with the following contents:

```bash
PORT="8080"
```

Run the server:

```bash
go build -o notely && ./notely
```

*This starts the server in non-database mode.* It will serve a simple webpage at `http://localhost:8080`.

You do *not* need to set up a database or any interactivity on the webpage yet. Instructions for that will come later in the course!

//* Adding updates for tests again & running the ci by pr


RUNNING TESTS
Our current CI doesn't do anything interesting.

A good CI pipeline typically includes unit tests, integration tests, styling checks, linting checks, security checks or any other type of automated test. If any of the tests fail, the build is considered broken and the developer is notified so they can fix it.
//* writing unit tests*//
// Like staticcheck, gosec is not part of the Go toolchain. We'll need to install it in our remote runner before we can use it.

//SECURITY REVIEW
Just because our codebase passes all of our tests, linters, and security checks doesn't mean it's "perfect" (or frankly even that it's "good").

These kinds of automated tests can help us eliminate ~80% of the most obvious bugs, stylistic anti-patterns, and security vulnerabilities, but they can't catch everything. We still need to take care to write good, secure code.

CI is an amazing tool to automate a lot of the stuff you'd manually check anyway. However, just because the checks pass doesn't mean your code is perfect. You still need to use your brain!



