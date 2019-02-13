---
short_name: step-1
name: Intro and Setup
step_number: 1
title: Into & Setup
---

## Welcome to the first step on your journey

You'll need a few things to get started!

1. [Visual Studio Code](https://code.visualstudio.com) - This is an EXCELLENT text editor. Highly configurable, with extensions for basically everything under the sun.
2. [Node JS](https://nodejs.org) - You'll want the LTS version. Install it, and make sure it's added to your PATH.
3. [Yarn](https://yarnpkg.com) - This is a package manager for nodejs, and the favoured tool of this tutorial. You might see references to `npm` as well. It serves the same purpose, but we'll be using `yarn`.
4. [Git](https://git-scm.com/) - Your bread and butter source control system. We'll be using it to save our work, basically.
5. [.NET Core 2.2 SDK](https://dotnet.microsoft.com/download) - We'll be using asp.net core as our server-side framework.


### Some Definitions

- **LTS: Long term support**. Sometimes, software is marked as extra stable, and will be supported for a bit longer. It's expected that LTS versions will be more stable, with the tradeoff that they won't get the same number of feature updates.
- **Source Control System**. Unlike a regular document, we care about previous versions of code **a lot**. It's very helpful to see the history of a file as it has evolved. It helps us to track down bugs, or just generally see how something has evolved over time. Git, and other source control systems, help us to save "snapshots" of code at a certain time. We can look at those snapshots, or even reset a file to a previous point in time.
- **Package manager**. All code we'll be writing is built using code that other people have written. Some of it is low level plumbing, some of it is helper functions that we don't really want to rewrite, some of it is code for interacting with other systems that a lot of people have poured a lot of time and energy into perfecting. We call this external code "packages" or "dependencies". Yarn helps us to manage our front-end dependencies. We'll see a similar package manager in the form of NuGet on the .NET side.