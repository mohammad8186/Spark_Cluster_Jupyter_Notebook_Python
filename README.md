# Spark Exercise Phase 2

This repository contains the implementation of **Phase 2 of Spark Exercise**, which was originally provided as a Jupyter Notebook and later extended for clarity and completeness. The exercise involves practical aspects of using Apache Spark for distributed data processing. Below is an overview of the exercise, its objectives, and the steps to set up and run the project.

## Overview
Apache Spark is an open-source, distributed computing system known for its ability to process large datasets efficiently using in-memory computations. This exercise aims to familiarize students with various Spark functionalities, including:

- Configuring and initializing a Spark session
- Working with Spark DataFrames and SQL
- Exploring Resilient Distributed Datasets (RDDs)
- Using user-defined functions for Spark tasks
- Comparing performance with and without caching

The implementation highlights the core differences between RDDs and DataFrames in terms of architecture, performance, and use cases, as well as the impact of various partitioning strategies.

## Objectives
1. Understand the architecture and capabilities of Apache Spark compared to traditional systems like Hadoop.
2. Explore and demonstrate:
   - Initialization of a Spark session
   - Data loading and transformations
   - SQL queries using Spark SQL
   - Optimizations with Catalyst and Tungsten engine
3. Analyze performance improvements using caching and partitioning strategies.
4. Compare **narrow** and **wide transformations** and their effect on execution times.

## Setup Instructions
Follow these steps to set up and run the project:

1. Clone the repository:
   ```bash
   git clone <https://github.com/mohammad8186/Spark_Cluster_Jupyter_Notebook_Python.git>
   ```

2. Navigate to the project directory

3. Start the cluster:
   ```bash
   bash master-build.sh
   ```

4. Open the Jupyter Notebook in your browser:
   ```
   http://localhost:8888
   ```

   Make sure you have a DNS or VPN if necessary.

5. Execute the notebook cells to explore the implementation and results.

## Key Features and Analysis

### 1. Data Processing Techniques
- **RDDs**: Low-level abstraction for distributed data processing with parallelism.
- **DataFrames**: High-level abstraction similar to SQL tables, optimized for performance and ease of use.
- **Spark SQL**: Provides SQL-like syntax for querying structured data.

### 2. Performance Optimization
- **Caching**: Demonstrated improvements in execution time when datasets are cached.
- **Partitioning**:
  - Default partitioning
  - Key-based partitioning
  - Custom partitioning

### 3. Transformations
- **Narrow Transformations**: Data dependencies within a single partition.
- **Wide Transformations**: Require data shuffling across partitions.

Performance comparisons and visualizations are included in the notebook to showcase the impact of these transformations.

## Report Highlights
The accompanying report delves into the following:

1. Differences between RDDs and DataFrames in terms of architecture and use cases.
2. Comparison of Spark SQL and DataFrame API capabilities, highlighting strengths and best use cases.
3. Explanation of partitioning strategies and their role in optimizing Spark jobs.
4. Analysis of performance with and without caching.

## Conclusion
This exercise demonstrates the power and flexibility of Apache Spark in handling large-scale data processing tasks. By exploring various optimization techniques, users can leverage Spark's full potential for efficient and scalable data processing.

Feel free to explore the notebook and provide feedback or suggestions!
