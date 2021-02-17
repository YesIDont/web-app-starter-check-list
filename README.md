# Web App Starter Check List
A list of steps to check when starting a new web app. Always keep in mind that:
- code starts simple and gets messy over time (always)
- code base should look as if it was created by one person (no exceptions)
- good programmer is polite to whoever will read he's code in the future, that means you want to write [Clean Code](https://www.youtube.com/watch?v=7EmboKQH8lM&t=4s)
- write your tests early, don't slack on it as it can backfire both on you as a programmer as well as on the business

## 1. Establish readme file like this one or similar.
It will act as entry point for any one new to the code base. It should hold the information of the following:
- stack: list containing frameworks, libraries and all tools being used to build the app
- paradigm: describe/list the way of the code. Is it functional? Procedural? Does it uses modules? Or mabe it's OOP?
- architecture: link/guide with description on what the app's structure will/should look like
- entry point: point your reader to the file that puts all of the code together, regardless if it's the usuall index.js / index.html or not.
- envs: links, explanations
- CSS: stack, do's and don'ts
- testing: tools, approach, do's and don'ts
- CI/CD, rules and pipeline description
- style guide: link/guide with detailed description of the code base style, also include selected approach to:
  - throwing Errors (in general using them is part of testing/documentation)
- IDE configuration: project specific IDE conf practices (e.g. priettier)
- point out to any other documentation related to that code base

Information about each of the above must be updated as soon as any of it changes. ALWAYS. Book your time to update your documentation.

## 2. Prepare first commit with initial setup
- install frameworks, libs and tooling required for the development
- configure testing tools
- if using Type Script: add types for all packages/libs/frameworks
- if it's in your job description: configure CI/CD
- configure git (or other service) repo:
  - create development, stage and production branches
  - set merges to be accept only from pull requests and block merging directly into any branch
  - setup team access
- push initial commit as first pull request and push it to code review. Rezist the temptation of creating initial configuration without code review! This is the foundation for the entire application. Anything that's missing or slipped your mind has a potential to create huge issue in future.
