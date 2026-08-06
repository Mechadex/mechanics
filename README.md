# Mechdex DB
This is the repository that contains all the game mechanics stored for Mechdex. It's free for anyone to contribute to. 

## Contributing
Each mechanic has a category that it's part of, and a unique "symbol" that looks mildly like a compound or periodic element.

Mechanics are stored in the following (highly inefficient but easy to write) way:
 - The repository contains one directory for every category, like `Abilities` or `Camera`.
 - Within each of these directories, one folder is made for each mechanic, named after the symbol. The folder contains a single file, `mechanic.yaml`.
 - The structure is like this:
 ```text
Main/
├── Category1/
│   ├── Symbol1/
│   │   └── mechanic.yaml
│   └── Symbol2/
│       └── mechanic.yaml
└── Category2/
    ├── Symbol3/
    │   └── mechanic.yaml
    └── Symbol4/
        └── mechanic.yaml
```


  So to create a new mechanic:
  1. Fork this repository. If you're not sure what that means, read up on a quick guide on how collaboration works on Github.
  1. Identify the right category.
  2. Within the category's folder, create a new folder with the name being the new mechanic's symbol, i.e., `Dj` or `Rc`. 
  3. Within this new folder, create a file `mechanic.yaml` (verbatim). Use another mechanic's `mechanic.yaml` as a template and fill in the details of this mechanic.
  4. Submit a pull request back to this repository. It'll be reviewed and merged.

## Exporting Data
You can run `generate_mechanics_table.py` to get a markdown representation of the entire data for further processing. The properties of the table are:
Name, Symbol, Category, Short Description, Long Description, Examples, Solved Problems, Drawbacks. 

## Credits
* Exporting data was implemented by [legibleguy](https://github.com/legibleguy).
