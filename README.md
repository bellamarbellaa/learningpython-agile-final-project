# My Python Learning Notes

This repo is where I keep my Python notes and practice notebooks. I use it to review what I have learned, try different examples, and practice analyzing data.

It is also part of my practice for IBM's **Getting Started with Git and GitHub** course, where I am learning to use commits, branches, pull requests, and GitHub.

---

## What I am learning

I started with Python basics, then moved on to classes, working with data, and making charts. Some notebooks use SpongeBob, Scooby-Doo, and Pokémon examples to make the concepts easier to follow.

| Notebook | What I practice |
| --- | --- |
| [Python Basics](python-basics.ipynb) | Variables, strings, operators, lists, dictionaries, and imports |
| [Python Intermediate](python-intermediate.ipynb) | Conditions, loops, lists, and string formatting |
| [Object Oriented Python](python-object-oriented.ipynb) | Classes, objects, methods, inheritance, and polymorphism |
| [NumPy](numpy.ipynb) | Arrays, calculations, indexing, filtering, and summaries |
| [Pandas](pandas.ipynb) | Working with tables, cleaning data, filtering, and grouping |
| [Matplotlib](matplotlib.ipynb) | Creating and customizing charts |
| [MySQL Analysis](PyMySQL-Pandas-MatplotlibAnalysis.ipynb) | Reading data from MySQL with PyMySQL, analyzing it with pandas, and making charts |
| [DuckDB Analysis](DuckDB-Pandas-MatplotlibAnalysis.ipynb) | Using SQL on a CSV, calculating salaries and bonuses, and plotting results |

---

## Analysis practice

I use NumPy for calculations, pandas to explore and clean data, and Matplotlib to turn the results into charts. The examples help me practice checking missing values, filtering rows, comparing groups, and understanding what the data shows.

I also practice SQL with MySQL and DuckDB. The MySQL notebook connects to an employees table, while the DuckDB notebook reads the employees CSV directly. Both let me work with the same kind of data and bring the results into pandas for analysis.

The [employees.csv](employees.csv) file has 1,000 practice records. I use it to explore salaries, bonuses, and teams. There is also a [pokemon.csv](pokemon.csv) file for data practice.

---

## How to use the notebooks

You can read the notebooks and their saved results on GitHub. To try the code, open a notebook in Jupyter or VS Code and run the cells from top to bottom. I usually change the values or queries to see what happens.

I use Homebrew on Mac to manage Python. For the data notebooks, install these packages in a notebook cell if needed:

```python
%pip install numpy pandas matplotlib duckdb sqlalchemy "pymysql[rsa]"
```

If an import still fails, restart the kernel and run the cells again.

The MySQL notebook needs a running MySQL server and the `employees` table in the `employees_python` database. Update the connection settings for your own setup and enter your password at the prompt. The DuckDB notebook uses the included CSV, so it does not need a server or login.

---

## Git and GitHub practice

I also use this repo to practice saving changes locally, pushing them to GitHub, working with branches, and opening pull requests. My notes are in [git-github-practice.md](git-github-practice.md).

---

## Learning materials

I learned from [Luke Barousse's Python Data Analytics Course](https://github.com/lukebarousse/Python_Data_Analytics_Course) and [Bro Code's YouTube channel](https://www.youtube.com/@BroCodez), then adapted the lessons and examples for my own practice, including the Pokémon examples.

The employee dataset is from [Prakhar Jadaun's Employee Data on Kaggle](https://www.kaggle.com/datasets/prakharjadaun/employee-data). I used Codex to help organize the notebooks, edit the notes, and check the code.

These notes are still a work in progress. I will keep adding to them as I learn.
