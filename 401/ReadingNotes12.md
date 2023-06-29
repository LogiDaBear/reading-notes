# Data Visualization

### What are the key differences between Matplotlib, Seaborn, and Bokeh libraries in terms of their features and use cases? Provide an example of a specific visualization that is more suitable for each library.
  - Matplotlib is a foundational library that offers extensive control over plotting

    Ex: A line plot showing the trends of stock prices over time.
      
  - Seaborn is focused on statistical visualizations with improved aesthetics

    Ex: A violin plot comparing the distribution of multiple variables across different categories, such as comparing the distribution of exam scores across different subjects.


  - Bokeh is ideal for creating interactive visualizations and web-based data applications. The choice of library depends on the specific requirements and goals of the visualization project.

    Ex: An interactive scatter plot showing the relationship between two variables, where hovering over the data points displays additional information about each point.

### In the Seaborn library, what are the main functions to create relational, categorical, and distribution plots? Briefly explain the purpose of each type of plot and provide an example use case.

- Relational plots:

  sns.relplot(): Creates a plot to visualize the relationship between two numeric variables, such as scatter plots or line plots.
  Purpose: Explore the relationship between continuous variables,   identify patterns, trends, and correlations.

    Example use case: Use sns.relplot() to create a scatter plot    examining the relationship between age and income, determining  correlation.

- Categorical plots:

  sns.catplot(): Creates plots to visualize categorical variable  distribution or relationships with numeric variables.
  Purpose: Explore categorical data, compare categories, understand distribution, and show relationships with numeric variables.
    Example use case: Use sns.catplot() to create a bar plot comparing average scores of students in different subjects, identifying highest or lowest scores.

- Distribution plots:

  sns.displot(): Creates plots to visualize single or multiple  variable distributions, including KDE plots and histograms.
  sns.kdeplot(): Creates a KDE plot to visualize the distribution of a single variable.
  Purpose: Understand data distribution, identify patterns, peaks,  outliers, and explore continuous variables' shape and spread.
    Example use case: Create a histogram using sns.displot() to     visualize the distribution of customer ages, identifying    significant age groups.

### Discuss the role of the Seaborn Cheat Sheet in a Python developer’s workflow. What are some key sections or elements featured in the cheat sheet that can help a developer quickly reference Seaborn functionalities?

The Seaborn Cheat Sheet serves as a quick reference tool, helping Python developers navigate the various functionalities and options available in the Seaborn library. It condenses important information and examples into a single document, making it easier for developers to efficiently utilize Seaborn for their data visualization tasks.

#### Plotting Functions:

`relplot()`, `catplot()`, `displot()`, and `kdeplot()`.
    Each function is accompanied by a brief description of its purpose and usage, making it easier to select the appropriate function for a specific visualization task.

- Categorical Plots:

    `barplot()`, `countplot()`, `boxplot()`, and `violinplot()`.
    It provides an overview of the function parameters and examples of how to customize the plots, such as adding error bars or changing color palettes.

- Relational Plots:

    `scatterplot()`, `lineplot()`, and `lmplot()`
    It showcases different plot types and demonstrates how to     incorporate additional dimensions using hue, style, and size    parameters.

## Things I want to know more about
Effectively using 'Data Storytelling' that enhances the experience of the data source