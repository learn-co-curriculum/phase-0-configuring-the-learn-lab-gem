# Configuring the learn-lab Gem

## Introduction

As you continue your journey into programming, you will learn to use many tools
to make your work easier that you only _sort of_ understand. Node packages, Ruby
gems, libraries, command-line applications, frontend frameworks, etc... many of
these tools are actually built out of _other_ tools, things you may never have
heard of. That is okay.

Thanks to the collective work of many programmers around the world, we're able
to tap in to a diverse ecosystem of tools. We don't need to know how they all
work together for them to be useful to us. You might one day know JavaScript
well enough to build your own version of [React]("https://reactjs.org/), but
you'll be able to use React long before you know how all the parts work. Many of
these tools are designed to solve problems so we can focus our energy and time
elsewhere.

We've already used a few tools to help us get started with programming. If you
recall from the previous installation instructions, we've installed NVM, the
Node Version Manager, which manages which version of Node you're using on your
computer. We've been using NPM, Node <strong>Package</strong> Manager, to run
local tests. We've also been using Git in the command line to interface remotely
with GitHub.

In this lesson, we're going to introduce another tool that will help us going
forward, the `learn-lab` gem.

## The `learn-lab` Gem

So, if all these tools we use are meant to solve problems, what problems does
the `learn-lab` gem solve?

Once you've pushed your solution up to GitHub, you then have to submit a link in
Canvas. The gem provides one final step. It verifies you got all your tests to
pass before submitting. We will have a new command called `learn-lab test`. This
new command will output a token that you should copy and paste into the comments
field of your submission.

**Important**: Throughout the course, you may see instructions in labs to run
`learn test` or `learn`. **You should disregard these instructions and run
`learn-lab test` instead.**

## Install the `learn-lab` Gem

**Note:** The instructions here assume you've successfully installed Ruby and
Node in the previous environment setup instructions.

To install the gem, run the following in your terminal:

```console
$ gem install learn-lab
```

Before we can use the gem, we'll need to configure it.

## Configure the Gem

### Action Item

1. Open your terminal
2. In your terminal run `learn-lab config`
3. Enter the same email you used for your Canvas login

## Using the `learn-lab` Gem

1. On this assignment's Canvas page, click the **Fork** button in the upper
   right corner of the page:

![fork buttton](https://curriculum-content.s3.amazonaws.com/fork-link.png)

You should notice a change in the button's behavior — rather than bringing you
to the fork page in GitHub, you'll be redirected to your repository _already in
the process_ of being forked.

2. Once your fork is ready, click the **Code** button and copy the **SSH**
   repository info by clicking the clipboard button.

![clone with SSH](https://curriculum-content.s3.amazonaws.com/phase-0/completing-assignments/clone-repo.gif)

**Note:** Make sure you're choosing SSH and not HTTPS.

3. In your terminal, navigate to where you'd like to put this repository
   locally, clone it down and navigate into the folder.

```console
$ git clone git@github.com:/phase-0-configuring-the-learn-lab-gem.git
$ cd phase-0-configuring-the-learn-lab-gem
```

4. run `npm install` to install all of the required packages.

You can now run `learn-lab test.` You should see the following:

![test passing message and token](https://curriculum-content.s3.amazonaws.com/phase-0/enterprise/configuring-the-learn-lab-gem/test-passing.png)

Note that, by cloning this assignment down, you've already passed the test! Go
ahead and commit your code and push it to GitHub.

The other thing to notice in the screenshot above is that, once all the tests
are passing (in this case it's just the one), you will also see a token printed
in the test output. This token indicates that you have successfully passed all
the tests for the lab.

Let's head back to the assignment page in Canvas. To submit the assignment, in
addition to submitting the link to your fork on GitHub, you will also submit the
token in the "Comments" box.

Specifically, you will need to:

1. Paste the link to your fork on GitHub in the "Website URL" box.
2. Go back to your terminal and select the entire token and copy it (using
   ctrl-C or cmd-C), then paste it in the "Comments" box in Canvas.
3. Click "Submit Assignment".

It should look something like this:

![submit repo url and token](https://curriculum-content.s3.amazonaws.com/phase-0/enterprise/configuring-the-learn-lab-gem/submit-assignment.png)

Each assignment will be different and will include instructions on what is
required to complete it. Some labs will have many tests. You can run
`learn-lab test` as many times as you'd like while working to solve these labs.

## Types of Assignments

For most assignments, you will go through the process we just walked through. In
our curriculum, these assignments are often referred to as **labs** — coding
lessons that include tests. There are a few other types of assignments, though,
that require slightly different submission steps:

- **Code-alongs:** These also require code, but will guide you through what
  needs to be written. There are no tests to pass. The process will be the same
  as for a lab, but there will be no token to submit.
- **Portfolio Projects:** For these assignments, you'll be building fully
  functional applications. Some guidelines and requirements will be provided,
  but it will be up to you to design and create your own app. These will
  eventually become the projects you showcase to potential employers! You will
  submit your projects in Canvas by submitting a link to your GitHub repo.
- **Blog Submissions:** Blogs are a required part of our Software Engineering
  courses. They help to develop your online presence and are a great way to
  reinforce the concepts you learn. You'll write your blog posts on a different
  platform, but submit links to them in Canvas.

## Conclusion

You've completed your first assignment using the `learn-lab` gem! You now know
how to work on and submit assignments going forward:

- Click the **Fork** button on the Canvas assignment.
- Once the assignment is forked, clone it down to your local machine.
- Complete any required work, then run `learn-lab test`.
- If all tests pass, you'll be provided a token.
- Push your work to GitHub.
- Enter the GitHub link in the "Website URL" box, and the token in the comments
  box, then click "Submit Assigment".

Equipped with this knowledge, you are now ready to tackle greater challenges!
