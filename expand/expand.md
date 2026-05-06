# Expand Section

## 1. Why JavaScript can be a pain point

Many developers believe JavaScript has issues because of its asynchronous behavior, loose typing, and the environment it runs in.

First, asynchronous behavior can be confusing. Code does not always run from top to bottom in a predictable order. For example, callbacks, promises, or async/await can make it harder to track when something actually executes. This often leads to bugs where data is not ready yet, or code runs earlier or later than expected.

Second, JavaScript is loosely typed, meaning variables can change types easily. While this makes coding faster, it can also introduce unexpected bugs. For example, adding two numbers stored as strings results in concatenation instead of arithmetic. These kinds of issues are easy to miss and can lead to incorrect results.

Lastly, JavaScript runs in the browser environment, which adds another layer of complexity. Developers have to deal with things like the DOM, browser differences, and network requests. These external factors make debugging harder compared to running code in a controlled environment.

## 2. Why JavaScript was designed this way

I think JavaScript was designed to be loosely typed because it needed to be simple and easy to use for web developers. At the time, the goal was to allow quick scripting inside browsers without requiring deep programming knowledge. Loose typing reduces the amount of code needed and makes the language more flexible.

Asynchronous features were likely added to improve performance and user experience. Browsers need to handle things like fetching data from servers without freezing the page. If everything ran synchronously, the website would become unresponsive while waiting for data. Asynchronous behavior allows multiple tasks to happen without blocking the main thread.

## 3. Compiled vs Interpreted languages

A compiled language translates the entire program into machine code before it runs. This usually makes execution faster, but requires a compilation step. Examples include C and C++.

An interpreted language runs code line by line at runtime, without compiling it ahead of time. This makes development faster and more flexible, but can be slower during execution.

JavaScript is generally considered an interpreted language, although modern engines use just-in-time compilation internally.

The benefit of JavaScript being interpreted is that it allows rapid development and immediate feedback. Developers can run code directly in the browser without compiling. However, the downside is that errors are only caught at runtime, and performance may be less predictable compared to compiled languages.

## 4. Why focus on vanilla JavaScript

The professor likely focuses on vanilla JavaScript so students can understand the fundamentals of how the language works. Frameworks often hide complexity, which can be helpful, but also makes it harder to debug or understand what is actually happening behind the scenes.

Learning vanilla JavaScript first helps build a strong foundation. It improves problem-solving skills and makes it easier to learn frameworks later. Developers who understand the basics can adapt more easily to different tools.

However, not learning frameworks has drawbacks. Frameworks are widely used in industry, and they provide structure, efficiency, and reusable components. Without them, building large applications can be slower and more difficult.

## 5. How this lab relates to the project

This lab helps build important skills that will be directly useful in the project. For example, using DevTools to debug code is essential when things do not work as expected. Understanding how asynchronous code works will help when dealing with APIs or fetching data.

The pipeline section is also important because it introduces automated testing and pull requests. This is something commonly used in real-world development, and it helps ensure code quality before merging changes.

Overall, this lab prepares me to write better code, debug more efficiently, and collaborate with others using tools like Git and pipelines. These are all skills that will be necessary when working on the project.