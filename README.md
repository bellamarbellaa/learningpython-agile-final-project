# My Python Learning Notes

My personal Python learning notes, organized into Jupyter notebooks with short explanations, code examples, and practice tasks. The notebooks cover Python basics, working with data, making charts, and using SQL through MySQL and DuckDB.

I use this repository to revisit concepts and try small examples. It also supports my practice for IBM's **Getting Started with Git and GitHub** course.

---

## How to use

Open a notebook on GitHub to read the notes and saved results. To try the code, open it in Jupyter or VS Code with notebook support, select your Python kernel, and run the cells from top to bottom. Change the example values to see how the results change.

I use Homebrew on macOS to manage Python. Install the packages you need in your notebook environment. The notebooks include setup notes; for the data analysis examples, run this in a code cell:

```python
%pip install numpy pandas matplotlib duckdb sqlalchemy "pymysql[rsa]"
```

Restart the kernel after installation if an import still fails. The Python basics, intermediate, and object oriented examples use Python's standard library.

---

## Notebooks

| Notebook | What it covers |
| --- | --- |
| [Python Basics](python-basics.ipynb) | Mac setup, imports, variables, strings, operators, lists, and dictionaries, using SpongeBob examples |
| [Python Intermediate](python-intermediate.ipynb) | Conditions, logical operators, lists, loops, and string formatting, using Scooby-Doo examples |
| [Object Oriented Python](python-object-oriented.ipynb) | Classes, objects, methods, inheritance, abstract classes, overriding, and polymorphism, using Pokémon examples |
| [NumPy](numpy.ipynb) | Arrays, dimensions, indexing, slicing, arithmetic, filtering, broadcasting, and random numbers |
| [Pandas](pandas.ipynb) | Series, DataFrames, CSVs, selection, filtering, grouping, and cleaning |
| [Matplotlib](matplotlib.ipynb) | Line, bar, pie, scatter, and histogram charts, styling, subplots, and saving figures |
| [MySQL Analysis](PyMySQL-Pandas-MatplotlibAnalysis.ipynb) | Connecting with PyMySQL and SQLAlchemy, reading employees into pandas, and plotting salaries and teams |
| [DuckDB Analysis](DuckDB-Pandas-MatplotlibAnalysis.ipynb) | Loading the employees CSV, SQL queries, bonus calculations, grouping, type conversion, and charts |

---

## Analysis Practice

These notebooks help me practice working with data, from calculations and cleaning to SQL queries and charts. Each notebook focuses on one tool, with examples I can change and explore.

**NumPy:** Work with arrays, select and filter values, perform calculations, and summarize numerical data.

**pandas:** Explore tables, check data types and missing values, clean labels, filter rows, and compare groups.

**Matplotlib:** Turn data into line charts, bar charts, scatter plots, pie charts, and histograms. Practice choosing labels, legends, and layouts that make results easier to read.

**MySQL and DuckDB:** Practice SQL using employee data. Connect to a MySQL table with PyMySQL and SQLAlchemy, or query the included CSV with DuckDB. Use the results to explore salaries, bonuses, and teams, then summarize them with pandas and create charts with Matplotlib.

The employee dataset contains 1,000 practice records. The notebooks use it alongside smaller examples to build analysis skills, rather than draw conclusions about a real workplace.

---

## Files included

The eight notebooks contain the lessons and saved outputs. [employees.csv](employees.csv) supports the employee analysis notebooks, and [pokemon.csv](pokemon.csv) is included for Pokémon data practice. The Pandas and Matplotlib notebooks also include small example datasets so they can run on their own.

[git-github-practice.md](git-github-practice.md) records my branch and pull request practice. I use Git to stage and commit changes locally, push them to GitHub, and pull remote updates back to my computer.

---

## Checks and scope

All eight notebooks have been run successfully, including the MySQL employee analysis and the DuckDB queries and charts. The MySQL notebook still requires a working local server and valid credentials when rerun. The DuckDB notebook uses the included CSV. The KaggleHub download and file exports are optional and are not run automatically.

These are learning exercises that I will continue to revise. Character details and example numbers are simplified for practice. The employee summaries demonstrate analysis techniques rather than conclusions about a real workplace.

---

## Learning materials

These notes draw on both [Luke Barousse's Python Data Analytics Course](https://github.com/lukebarousse/Python_Data_Analytics_Course) and [Bro Code's YouTube channel](https://www.youtube.com/@BroCodez). I adapted the lessons and examples, including Pokémon examples, for my own practice. The employee dataset used in the DuckDB material is available through [Prakhar Jadaun's Employee Data on Kaggle](https://www.kaggle.com/datasets/prakharjadaun/employee-data).

The notebooks were organized, edited, and checked with help from Codex.
