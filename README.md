# Data Journalism Template for Transparency!

## Motivation
* To encourage data journalists to make their process transparent
* To begin to standardize how transparency might be achieved – what should and not be included, and how information should be organized so curious parties can know what to expect and where to find things.

This [blog post](https://blog.ouseful.info/2017/01/25/data-journalism-units-on-github/) talks about tools in data journalism transparency with a great list toward the bottom with examples in practice. You'll see that there is no consensus as to how to share information, what information to share, and the format of that information, meaning that each time you look at a project, you have to figure out where everything is, and what is available.

### Benefits to standardizing project structure for transparency
* Less of a chore if it has already been figured out - how to organize and what to include
* Organized, properly documented projects are easier
  - to refer back to,
  - to train new journalists,
  - for the public to explore and scrutinize

The current repository is an attempt to construct an organized, standardized "Data Journalism Project" structure for sharing the analysis and data with others - other journalists, the public, government bodies etc. The directory structure is partly inspired by two CookieCutters: [Reproducible Science](https://github.com/mkrapp/cookiecutter-reproducible-science) and [Data Science](https://github.com/drivendata/cookiecutter-data-science) by the same author.
Data Journalism stories tend to be one-offs, and difficult or impossible to replicate by inputting data from a different city or industry, for example, so creating a new organization structure seemed to make sense to me, rather than applying one of these existing projects directly. I also wanted to make it as lightweight as possible, since it is already going to feel like a lot of extra work to implement, until it becomes more familiar and routine.

### A suggested directory structure

The directory structure might look a bit like this:

```
├── AUTHORS.md        <- Everyone contributing to the story.
├── LICENSE           <- Select a license for the analysis and/or the data.
├── README.md         <- The top-level README for developers using this story.
├── data
│   ├── interim       <- Intermediate data that has been transformed, filtered or cleaned.
│   ├── processed     <- The final data sets for analysis.
│   └── raw           <- The original data, read only.
│
├── notebooks         <- Jupyter notebooks and analysis scripts. If there are several sequential
│                        scripts or notebooks, consider naming numerically, like `0_data-exploration.ipynb`.
│
├── references        <- Data dictionaries, manuals, notes, sources, articles and other explanatory materials.
│
├── reports           <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures       <- Generated graphics and figures to be used in reporting
│
├── requirements.txt  <- The requirements file for reproducing the analysis environment, e.g.
│                        generated with `pip freeze > requirements.txt`. Alternatively you can type in software,
│                        libraries, and versions yourself.
│
├── .gitignore        <- List of files and folders that you do not want tracked by git and/or published online.
│
│
└──  keys.txt         <- Contains all keys or access tokens for APIs, servers, databases etc that should not be shared.

```

## Directory Description

#### `LICENSE`
No license leaves your project code and data in legal limbo. If you don't mind people using your analysis or software, you'll need a license. A popular license is the [Creative Commons ShareAlike license](https://creativecommons.org/licenses/by-sa/4.0/). You can also check out [this page](https://choosealicense.com) for software-style licenses that can be used for non-software projects, and [these](https://choosealicense.com/non-software/) options for non-software type work.

#### `README.md`
You would write a describe the project with link to the story and subheadings like:
* blah
* foo
* Ra

You can find out how to write markdown [here](https://guides.github.com/features/mastering-markdown/)

### `data`

## Instructions
Take a look at the `Example` branch to see what a project might look like – what information is provided in each section, formatting, etc.

To use this for your own project, either recreate the directory tree by hand, or clone this project, copy contents to new project or delete the `.git` folder, type `git init` and fill the project in!

## Future plan
Once I've tested it out, gotten feedback and made necessary adjustments, make a CookieCutter :smile:

## Contributing

I welcome your feedback and suggestions to jastark1@gmail.com !

### Installing development requirements
`pip install -r requirements.txt`
