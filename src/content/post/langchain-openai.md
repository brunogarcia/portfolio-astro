---
publishDate: "2023-02-04T16:06:36.571Z"
title: "Research about LangChain and the API of OpenAI"
description: "The main goal of both projects is to research about the LangChain library and the API of OpenAI using the Titanic SQLite database."
tags: ["openai", "langchain", "react", "typescript"]
---

## How is it working?

On both cases, I'm using the **SQL Database Chain** of LangChain.

Also I'm using [Next.js](https://nextjs.org/) to create a simple web application that allows me to interact with the database in a natural language way.

## Github

Check out the source code on Github.

- [Titanic Jupiter Notebook](https://github.com/brunogarcia/langchain-titanic-sqlite)
- [Titanic Next.js App](https://github.com/brunogarcia/nextjs-langchain-titanic-sqlite)

## Tools

- [OpenAI API](https://openai.com/blog/openai-api)
- [Python LangChain](https://python.langchain.com/) and [Javascript LangChain](https://js.langchain.com/) libraries

## Database

The table is called `titanic` and has the following columns.

🥳 Amazing: even the this table was created using natural language:

> "Give the column name, data type and description of the table titanic in markdown format"

| Column Name | Data Type | Description                           |
| ----------- | --------- | ------------------------------------- |
| PassengerId | TEXT      | Unique identifier for each passenger  |
| Survived    | TEXT      | Whether the passenger survived or not |
| Pclass      | TEXT      | Passenger class                       |
| Name        | TEXT      | Passenger name                        |
| Sex         | TEXT      | Passenger gender                      |
| Age         | TEXT      | Passenger age                         |
| SibSp       | TEXT      | Number of siblings/spouses aboard     |
| Parch       | TEXT      | Number of parents/children aboard     |
| Ticket      | TEXT      | Ticket number                         |
| Fare        | TEXT      | Ticket fare                           |
| Cabin       | TEXT      | Cabin number                          |
| Embarked    | TEXT      | Port of embarkation                   |

## Answering the questions with natural language

The app and the notebook are able to answer the following questions in natural language:

1. How many passengers survived?
2. How many passengers were in each class?
3. How many passengers survived/died within each class?
4. What was the average age of survivors vs non-survivors?
5. What was the average age of each passenger class?
6. What was the average fare by passenger class? By survival?
7. How many siblings/spouses aboard on average, by passenger class? By survival?
8. How many parents/children aboard on average, by passenger class? By survival?

### Example #1: How many passengers survived?

```html
342 passengers survived.
```

### Example #2: How many passengers were in each class?

```html
There were 216 passengers in first class, 184 passengers in second class, and 491 passengers in
third class.
```
