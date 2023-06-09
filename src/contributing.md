# Contributing

## Prerequisites

- Version control system Git

  - Windows: [Download](https://git-scm.com/download/win) and install Git
  - Mac: `$ brew install git`
  - Linux: Use your package manager, for example `$ apt install git` , `$ dnf install git` or `$ pacman -S git`. Keep in mind that your distribution might use a different one.

- A file editor of your choice

  - If you do not have a file editor installed, online editors such as [StackEdit](https://stackedit.io) or GitHub's built-in one will work as well

- A user account on [GitHub](https://github.com/)

> **NOTE:** If you don't have a computer, or your computer does not allow installing this software (i.e. school computers) but would still like to help, check [Contributing with GitHub alone](./contributing-2.md)

Optional, but heavily recommended:

- Rust package manager Cargo and the mdbook crate
  - [Download](https://www.rust-lang.org/tools/install) and install using these instructions
  - Install the mdbook crate using `$ cargo install mdbook`

## Creating your fork

In terms of Git repositories, a fork is a separate version of a project, usually for another user to make changes and create merge requests. That's exactly what we'll do!

Visit [the original repository](https://github.com/IdleRPGBot/idlerpg-guide) and find the "Fork" button. Click it, select your account and GitHub will create a fork for you.

The fork will have its own URL, being `https://github.com/<your username>/idlerpg-guide`. To copy it, find the green "Code" button and copy the URL.

Congratulations, you now have your own fork of this book! Now we need to get it onto your computer.

## Cloning the repository

To start writing contents, you first need to get your own copy of - what we refer to as "clone" - this book.

To do so, on your computer, navigate to a directory you want to store the book in. Next, run the following command in your terminal:

```sh
$ git clone git@github.com:<your username>/idlerpg-guide.git
```

_Make sure to replace \<your username\> with your actual username. In my case, it would be `git@github.com:Gelbpunkt/idlerpg-guide.git`._

This will create a new directory named "idlerpg-guide". In it, you will find the book's files. The actual contents of the book are found in the `src` directory.

Here, you can add new files, edit existing ones, etc.

## Adding new pages

If you wish to add new pages, you can simply create a new file in the `src` directory. The file should end in `.md` so that the book knows this is a file to add.

Once you have done this, **add the newly added page to `SUMMARY.md`!** This is essential for the book to properly work. The file acts like a table of contents.

Each page should have a title, you can do so by adding `# Page Title` to the bgeinning of the file. In Markdown, this is a headline.

Of course, not only the page's title will be formatted according to Markdown; the entire page is!

_But what is Markdown?_ Markdown is a convenient way to format text. You might even have used markdown without knowing it!

In markdown, two asterisks around a bit of text \*\*like this\*\* will make the text bold **like this**!

Markdown is used to create **emphasis** on certain bits of text, we encourage you to highlight certain parts. For a markdown cheatsheet, visit [this page](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

## Making changes

If you want to make a change to a page, i.e. correct text or write some new blocks, simply open the right file in your file editor and change the text.

There are no further things you have to pay mind to.

## Previewing changes

_NOTE: This will be easier if you have cargo and the mdbook crate installed. If you don't have rust or the mdbook crate installed, you can preview your changes after committing changes. More on that in the next section._

If you want to check what your changes look like before you save them, mdbook offers options.

Open your terminal in the project directory `idlerpg-guide` and enter the following:

```sh
$ mdbook build
$ mdbook serve
```

This will run a webserver for the files. You can open `http://localhost:3000` in your webbrowser to view the generated book while it is serving.

## Saving (committing) and uploading (pushing) your work

Saving your work using Ctrl+S is not enough if you want to publish it; you'll want to _commit_ it, so that the version control system Git knows this is a new version.

To do this, open your terminal in the `idlerpg-guide` directory and use the following commands:

```sh
$ git add ./src/page.md
$ git commit -m "Commit message here!"
$ git push
```

- `$ git add` marks the file(s) as ready to commit. This is useful in projects, where you may have changes in multiple files, but only want to commit a few.
- `$ git commmit` commits the files in git. The `-m "Commit message here!"` is known as the commit message. In it, you should describe briefly what you did.
- `$ git push` uploads, or pushes the commited files to a remote repository, in this case, your repository on GitHub. From there, you can create a merge request to have your changes implemented into our project.

Commited files are different to saved files in that any commit exists simultaneously. If you save a file, make changes and save again, the old save is gone, but different commmits can be accessed at all times.

Make sure to replace `./src/page.md` with the file path to the newly added and/or changed files. `SUMMARY.md` should always be included if you created a new page.
Also replace `Commit message here!` with a short note on what you did, i.e. `Added new page contributing.md`. Commit messages have a maximum of 50 characters, so keep it short and spicy!

After pushing, a CI (continuous integration) on GitHub will build the html files and provide a preview for you. To view this, make sure you have the previews enabled by going to the repository settings on GitHub, selecting the "Pages" tag and selecting the `gh-pages` branch as the deployment source.

![image](img/github_pages_setup.png)

When you push your changes, you will now be able to view a preview at https://yourusername.github.io/idlerpg-guide.

_Of course, previewing changes this way is a bit tedious, so we recommend getting rust and the mdbook crate and using the method mentioned above._

## Creating a pull request

Great! Your files are now uploaded, we're ready to make the changes official.

Head to your repository on GitHub, the URL is `https://github.com/<your username>/idlerpg-guide`.

At the top of the page, you should already see a hint saying that you pushed changes with a "create pull request" button next to it. Click it!

Feel free to explore this page to your liking, but the important part is giving your pull request a title and a description.

It is completely fine to use the commit message as the pull request's title, as long as we know what the changes are.

In the description, you should add your name (_so we can add you to the book authors_), among other things you deem important.

Finally, hit the "open pull request" button! We'll take over from here. But don't forget to check back if we have reviews for your changes, you might be asked to change parts with a new commit.
