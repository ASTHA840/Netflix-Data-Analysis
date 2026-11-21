# 🎬 Netflix Content Analysis Using SQL Server

**A SQL data analysis project by Astha Gautam**

## 🛠️ Tools and Technologies Used

| Technology | How it is used |
| --- | --- |
| **Microsoft SQL Server** | Database platform used to store and query the Netflix titles dataset |
| **T-SQL (Transact-SQL)** | SQL language used to filter, group, count, rank, and summarize records |
| **SQL Server Management Studio (SSMS)** | Tool used to connect to SQL Server, write queries, and view query results |

The project demonstrates `GROUP BY`, aggregate functions, window ranking with `RANK()`, date functions such as `DATEADD()` and `YEAR()`, text matching with `LIKE`, cast parsing with `STRING_SPLIT()` and `TRIM()`, `CROSS APPLY`, and conditional logic with `CASE`.


> Explore the Netflix titles catalog with SQL: compare Movies and TV Shows, examine ratings and countries, analyze genres and cast, and review title metadata.

## 📌 Project at a Glance

| | |
| --- | --- |
| **Project type** | SQL data analysis |
| **Domain** | Streaming media catalog |
| **Database** | Microsoft SQL Server (`netflix`) |
| **Query language** | T-SQL |
| **Main table** | `netflix_titles` |
| **Analysis questions** | 15 |
| **Query editor** | SQL Server Management Studio (SSMS) |

## 🎯 Project Overview

This project analyzes a Netflix titles dataset stored in a table named `netflix_titles`. It uses SQL queries to explore catalog metadata, including content type, title, director, cast, country, date added, release year, rating, duration, genre, and description.

The goal is to practice SQL-based data exploration and turn a set of questions into useful catalog summaries. The analysis describes records in the dataset; it does not measure views, popularity, or audience preferences.

## ❓ Problem Statement

A content catalog contains many records and different types of information. Reviewing it manually makes it difficult to compare Movies with TV Shows or summarize titles by rating, year, country, genre, director, or cast. This project uses T-SQL queries to answer these questions in a structured way.

## 🧭 Project Workflow

```mermaid
flowchart LR
    A[Netflix titles dataset] --> B[netflix_titles table]
    B --> C[Review and prepare data]
    C --> D[Run 15 T-SQL analyses]
    D --> E[Review query results]
    E --> F[Summarize findings and recommendations]
```

## 📄 Dataset

The project uses a Netflix titles dataset loaded into `netflix_titles`. The report references these fields:

| Field | Description |
| --- | --- |
| `show_id` | Identifier for a title record |
| `type` | Content type, such as Movie or TV Show |
| `title` | Title name |
| `director` | Director information |
| `cast` | Cast names |
| `country` | Country or countries associated with the title |
| `date_added` | Date the title was added to the catalog |
| `release_year` | Original release year |
| `rating` | Content rating |
| `duration` | Movie runtime or number of TV seasons |
| `listed_in` | Genre or category information |
| `description` | Title description |

**Dataset source:** Add the original dataset source or download link here. The supplied report and SQL script do not specify it.

## 🗃️ Database Architecture and ER View

The project uses one main table. The supplied SQL does not define related tables or foreign-key relationships, so the data model is a single entity rather than a multi-table relational design.

```text
netflix database
└── netflix_titles
    ├── show_id
    ├── type
    ├── title
    ├── director
    ├── cast
    ├── country
    ├── date_added
    ├── release_year
    ├── rating
    ├── duration
    ├── listed_in
    └── description
```

## 🧹 Data Cleaning and Preparation

The SQL script includes a step that deletes records where `country` is null. This changes the table and can affect later query results. Keep a backup or use a working copy before running the deletion.

Before analysis, confirm that the expected columns and data types are present. Pay attention to missing values and to fields such as `country`, `listed_in`, `cast`, and `duration`, which may contain multiple values or values stored as text.

## 📊 Analysis Questions

1. Count Movies versus TV Shows.
2. Find the most common rating for Movies and TV Shows.
3. List Movies released in 2020.
4. Find the top five countries by content count.
5. Identify the longest Movie.
6. Find content added in the last five years.
7. Find titles by director Rajiv Chilaka.
8. List TV Shows with more than five seasons.
9. Count content by genre/category.
10. Find the top five years for Netflix additions in India.
11. List documentary Movies.
12. Find content without a director.
13. Count Salman Khan Movies in the last ten years.
14. Find the top ten actors in India-related Movies.
15. Categorize descriptions using the keywords “kill” and “violence”.

## 📈 Answers and Insights

1. **5,189 Movies; 147 TV Shows.**
2. **TV-MA — Movies: 1,741; TV Shows: 81.**
3. **Visible titles:** Omo Ghetto: the Saga; Shikara; Really Love; The Old Ways; La diosa del asfalto; Quam's Money; Sanitation Day; Milkwater; Har Kisse Ke Hisse: Kaamyaab; Rattlesnake - The Ahanna Story; Voiceless.
4. **United States (1,849); India (875); United Kingdom (183); Canada (107); Spain (91).**
5. **The School of Mischief — 253 minutes.**
6. **Recent title records are shown; the screenshot does not show the complete list or total.**
7. **3 Movie records.**
8. **9 TV Show records; durations shown range from 6 to 9 seasons.**
9. **Top visible:** Dramas, International Movies (336); Stand-Up Comedy (286); Comedies, Dramas, International Movies (257); Dramas, Independent Movies, International Movies (243); Children & Family Movies, Comedies (179).
10. **2018 (325); 2019 (198); 2020 (179); 2017 (140); 2021 (89). Average: 156.**
11. **Documentary Movie records returned; full list and total are not visible.**
12. **No rows shown in the supplied result screenshot.**
13. **1 Movie.**
14. **Anupam Kher (40); Shah Rukh Khan (34); Naseeruddin Shah (31); Om Puri (29); Akshay Kumar (29); Amitabh Bachchan (28); Paresh Rawal (28); Boman Irani (27); Kareena Kapoor (25); Ajay Devgn (21).**
15. **Good (5,108); Bad (228).**
## 🔍 Key SQL Logic

- **Filtering:** Select records that match a content type, year, director, cast name, country, or keyword.
- **Aggregation:** Use `COUNT()` and `GROUP BY` to summarize catalog records.
- **Ranking:** Use `RANK()` to find the most common rating within each content type.
- **Date analysis:** Use date functions to define time periods and group additions by year.
- **Text analysis:** Use `LIKE` to search descriptions and metadata fields.
- **Cast analysis:** Split comma-separated cast text into individual names before counting.
- **Conditional categories:** Use `CASE` to assign a label based on description keywords.

## 📈 Business Insights and Recommendations

The displayed results show that Movies greatly outnumber TV Shows, TV-MA is the most common rating for both types, and the United States has the highest country count. India additions peak in 2018 in the shown results. Add further recommendations after reviewing complete result grids.
## 💼 Skills Demonstrated

- Writing T-SQL queries to answer analytical questions
- Filtering and aggregating records
- Using window functions for ranking
- Applying date and string functions
- Splitting multi-value text fields for analysis
- Reviewing data quality and query limitations
- Presenting query results in a structured report

## ⚠️ Interpretation Notes

- The country cleanup step deletes records with missing country values. Preserve a source copy before running it.
- The director query returns `type` and `director`, but does not return the title name. Add `title` to the selected fields if the goal is to list matching titles.
- The TV show duration condition compares text. Extracting the numeric season count first would be more reliable.
- The India year query uses `YEAR(date_added)`, although its output column is named `release_year`. It describes the year the title was added, not the original release year.
- Country and genre fields may store multiple values together, so grouping the entire field may count combinations rather than each individual country or genre.
- The “Bad” and “Good” description labels are based only on keyword presence. They are not a content-safety or age-suitability assessment.
- The Salman Khan query uses the current SQL Server year, so its ten-year cutoff changes over time.

## ✅ Conclusion

This project uses Microsoft SQL Server and T-SQL to explore Netflix catalog metadata through 15 analysis questions. It demonstrates practical SQL skills in filtering, grouping, counting, ranking, date analysis, and text processing. The final conclusions should be based on verified query outputs and should account for the dataset and query limitations described above.










