# Code Class Template

The Code Class Template is a way to organise all information of a code class in one place. The template
consists of an index file with information on the code class, a list of exercises, the presentation
of the code class and the stream of the code class.

## Getting started

This project is hosted as a Voorhoede Git repository. Clone it:

``` bash
$ git clone git@github.com:voorhoede/code-class-template.git
```

Install dependencies:

``` bash
$ npm install
```

Start server & watch files:

``` bash
$ npm run start
```

This wil build the project, start the server and start the watcher. The project is
available on [localhost:3000](http://localhost:3000). The watcher task will automatically
build assets, styles and views. The server will be reloaded on every change.

## Set up code class

When you set up your code class, copy this repository and follow these steps:

- [Add code class information](#add-code-class-information)
- [Create exercises](#create-exercises)
- [Create presentation](#create-presentation)
- [Create YouTube stream](#create-youtube-stream)
- [Cleaning up](#cleaning-up)

### Add code class information

Add the title of your code class to the following file (see the TODO comment):

```
src/views/_base/base.html
```

Add any context or other general information relevant to your code class to the following file (see the TODO comment):

```
src/views/index/index.html
```

### Create exercises

Every exercise and solution to an exercise must be placed in a folder in the views folder, for example:

```
views
├── _base
├── exercise-1
├── exercise-1-solution
├── exercise-2
├── exercise-2-solution
└── index
```

For every exercise and it's solution a page will be generated. Add the links to the exercises to
the list in the following file (see the TODO comment):

```
src/views/index/index.html
```

An example exercise and solution file can be found in the views folder. An exercise file consists of
different [Nunjucks](https://mozilla.github.io/nunjucks/) blocks:

Block | Description
---|---
`navigation` | Navigation to the index of the code class and to the answer of the exercise
`introduction` | Introduction to the exercise or a description of the exercise
`html` | The HTML necessary for the exercise
`styles` | The CSS necessary for the exercise
`scripts` | The JavaScript necessary for the exercise

Add the content for your exercises (see the TODO comments).

### Create presentation

A [presentation template](https://docs.google.com/presentation/d/1ZcTSzPasxAO5MOfTYDRLKbN4ankG2ZS80SU4qwpXGFM/edit?usp=sharing) is available in the Google Drive of De Voorhoede. Create your presentation in Google Slides using this template.

After you created your presentation, attach it to your project. In Google Slides, click on:

```
File > Publish to web... > Embed > Publish
```

Copy and paste the generated url into the following file (see the TODO comment):

```
src/views/index/index.html
```

### Create YouTube stream

Set up the YouTube stream using the [streaming manual](https://www.dropbox.com/s/td9dc64mux3fggm/_streaming-manual.pdf?dl=0).
Copy and paste the generated url into the following file (see the TODO comment):

```
src/views/index/index.html
```

### Cleaning up

Add the title and any context or other information relevant to your code class to this README.

Remove the section "Set up code class" from this README (and keep the section "Getting started").
