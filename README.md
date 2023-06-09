# Tiny Shop Exercise - PostgreSQL and Jupyter Notebook

## Introduction

To practice my SQL skills, I chose this SQL Case Study by [Data In Motion](https://d-i-motion.com/). The case study can be found [here](https://d-i-motion.com/lessons/customer-orders-analysis/). It's a fairly easy exercise that contains 10 questions that need to be answered using SQL.

However, to accelerate my learning, I also wanted to test out the connection between Python, Jupyter Notebook and PostgreSQL, because I had never tried that.
## Dependencies

To run this code, make sure you have the following packages:
`ipython-sql`
`sqlalchemy`
`python-dotenv`

You can also create a database called `tinyshop` in your PostgreSQL instance as I have not included that in the notebook. The code includes a connection string to the locally hosted PostgreSQL database with credentials stored in .env, but feel free to change the connection parameters.

## Process

1. First of all, I installed PostgreSQL on my Mac using Homebrew.
2. I then set up a new SQL database called tinyshop by running `CREATE DATABASE tinyshop;`
3. I had already installed the Anaconda distribution of Python, so I went ahead and created a new virtual Python environment by running `conda create -n newenv python`. Virtual environments are really important because different projects will have different dependencies.
4. There was one package that I wanted to test in this case, and that was `ipython-sql`, so I ran `conda install ipython-sql`. This gives us the ability to use the %%sql cell magic and %sql line magic commands, so we can query the data from our database easily. We can also use functions from `sqlalchemy`, but I think in this case we won't need them just yet.
5. In the code, you will see me store the PostgreSQL username and password in the `.env` file and then importing the `dotenv` and `os` Python packages. In the case of my locally-hosted Postgre database, it's maybe not that important, but I decided this was a a good opportunity to get used to this practice - in the future, I certainly don't plan to post any login information publicly on GitHub. :)
6. I have also tried to use some automatic formatting of my SQL code in the cells with %%sql, but haven't found a satisfactory solution yet.
## Some notes:

This being my first "project", I believe I have learned a lot especially when it comes to using PostgreSQL (I originally learned SQL using MySQL and I also sometimes use BigQuery), connecting to it from Jupyter Notebook, setting up Jupyter Notebooks in VS Code and creating virtual python environments.

Also I did get a chance to practice SQL, although these exercises where all data is already clean and loaded into the database are probably a bit too easy compared to real-world problems!