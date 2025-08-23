# Why most Java projects don't use commit hooks

#### And why that's actually a good thing

---

I heard the term “commit hooks” or “Git hooks” many years ago. It’s especially emerged in the JavaScript community, where fancy and shiny things get a lot of attraction from developers. I used to apply it in some of my personal projects to trigger ESLint and Prettier when I commit. At that time, everything was fine and the only thing I didn’t like was it added a lot of dependencies (Husky and Lint-staged, I’m looking at you two).

But my professional work started with Java, a much more mature ecosystem compared to JavaScript. Java refreshed my mind and I realized many shiny things I have ever seen were just simply unncessary. And you know, commit hooks are included.

## 1. Why commit hooks

Lots of dependencies:

Husky, lint-staged

You know where things have gone too far? Check this yourself.

## 2. But how Java can get rid of commit hooks

CI pipeline

A super power command: mvn clean install

Remember to run the command

https://github.com/tonghoangvu/test-blog/blob/main/Screenshot%202025-07-11%20000450.png

![Alt text](https://github.com/tonghoangvu/test-blog/blob/main/Screenshot%202025-07-11%20000450.png)
