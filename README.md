# Data Journalism Template for Transparency - Example!
* [Story title]() linked to the online story.
* [Link to data]() if there was data located elsewhere (not in this repository on GitHub due to size restrictions of 500 MB).
* [CODA-BR 2017 slides]() "Thinking About Algorithmic Accountability" keynote on algorithmic transparency for tech and for journalism.

## Motivation
To provide a basic example of making data driven journalism (DDJ) transparent to readers, other journalists and government or civic-minded people for my workshop ["How to implement editorial transparency in data journalism"](http://coda.escoladedados.org/#programação) at the 2nd CODA•BR data journalism conference in São Paulo, Brazil 2017.

The example dataset is taxi trips in Washington, D.C. from their [open data portal](http://opendata.dc.gov/datasets?q=taxi).



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
