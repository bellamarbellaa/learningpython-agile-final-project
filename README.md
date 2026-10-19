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

## MySQL and DuckDB

These are two ways to analyze employee data. Both use pandas for tables and Matplotlib for charts.

**MySQL:** The notebook connects to a running MySQL server through PyMySQL and SQLAlchemy. It uses the `employees` table in the `employees_python` database. Import [employees.csv](employees.csv) into that table using MySQL Workbench, then check the host, port, and username in the notebook. The current settings are `127.0.0.1:3306` and username `root`. Enter your own password at the private prompt. Passwords are not stored in the notebook.

**DuckDB:** The notebook reads [employees.csv](employees.csv) directly. It needs no server or login. It creates a temporary database, runs SQL, and converts the results to pandas. Closing the connection removes the temporary tables; the CSV remains available. To keep tables between sessions, connect to a `.duckdb` file instead.

The employee CSV contains 1,000 practice records with salary, bonus, team, and other columns. The DuckDB notebook uses this local file; the MySQL notebook reads the table you imported into your server.

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

These notes draw on lessons from [Bro Code's YouTube channel](https://www.youtube.com/@BroCodez), including Python basics and Pokémon examples. I adapted the examples for my own practice. The employee dataset used in the DuckDB material is available through [Prakhar Jadaun's Employee Data on Kaggle](https://www.kaggle.com/datasets/prakharjadaun/employee-data).

The notebooks were organized, edited, and checked with help from Codex.
