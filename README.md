# Cloud Computing Project: Search Engine with Inverted Index

## Objective

The project involves the creation of an **inverted index** starting from a collection of files. The goal is to build a scalable and extensible system capable of indexing texts and answering textual queries.

## Inverted Index Example

```
cloud      doc1.txt:1  doc2.txt:1
computing  doc1.txt:1  doc2.txt:1
is         doc1.txt:1
important  doc2.txt:1
```

## Main Requirements

- Install **Hadoop in fully distributed mode**.
- Implement two versions of the inverted index:
  - One using **Hadoop (Java)**
  - One using **Spark (Python)**
- For each detected word, the inverted index output must include:
  - The names of the files where the word appears
  - The number of occurrences of the word in each file

- Implement **combiner** logic
- Use the `setup()` and `cleanup()` methods, if appropriate
- Build a simple **non-parallel search engine in Python** that:
  - Receives a text query
  - Returns **only the file names** that contain **all** query terms (it must not indicate the number of occurrences)

- Use a collection of files of choice (e.g., articles, books, web pages), varying in size from **a few KB to several GB**
- Perform a **comparative performance evaluation**, collecting:
  - Execution time
  - Memory usage
  - Other relevant indicators
- Draft a **technical report** containing:
  - Pseudocode of the MapReduce solution in Hadoop
  - Description of the datasets
  - Experimental analysis

## Additional Requirements

- Implement **in-mapper combining** logic
- Develop a **non-parallel version in Python** for building the inverted index 
- Increase the **number of reducers** and collect execution-related statistics
