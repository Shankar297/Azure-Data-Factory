# Azure Data Factory Full Course (Beginner to PRO) - Full Notes

Welcome to this comprehensive summary of the YouTube video **"Azure Data Factory Full Course (From Beginner to PRO) | ADF Real-Time Scenarios"** by Ansh Lamba. This README serves as a structured companion to the tutorial and walks you through all the essential concepts, tools, and real-world scenarios.

---

## 🎯 Course Objective
To master Azure Data Factory (ADF) from scratch, including hands-on real-time use cases and interview-ready scenarios. By the end of this course, you'll:

- Understand ADF fundamentals
- Work with pipelines, linked services, datasets
- Build ETL/ELT pipelines
- Use data flows and real-time triggers
- Integrate external APIs, Data Lake, and other services

---


## 🧠 What is Azure Data Factory?
ADF is a **cloud-based ETL/ELT tool** used to orchestrate and automate data movement and transformation.
- It connects to various **data sources** (SQL, API, files, etc.)
- It moves data between **source and destination**
- It performs **transformation** using **Mapping Data Flows** (Spark under the hood)

---

## 🔗 Core Concepts
### Linked Service
- A **connection** to a data source/destination (e.g., SQL DB, Azure Data Lake, HTTP API)

### Dataset
- Defines **which data** to work with (e.g., a specific table, file, or folder)

### Pipeline
- A group of **activities** used to perform a complete data workflow

---

## 📂 Resources Used in Tutorial
### 1. **Azure Storage Account** (configured as Azure Data Lake Gen2)
- Source & destination containers
- Real folder structures

### 2. **Azure Data Factory Instance**
- Pipelines with multiple activities

### 3. **GitHub (External API)**
- Pull data directly from a hosted CSV file

---

## 🔄 Core Activities Covered

### ✅ Copy Activity
- **Use Case**: Move data from Source (Data Lake/HTTP) to Destination (Data Lake)
- **Components**: Source & Sink datasets, linked services

### ✅ Get Metadata Activity
- **Use Case**: Get info (e.g., file names) about a folder
- **Output**: Array of files, last modified dates, etc.

### ✅ If Condition Activity
- **Use Case**: Filter files based on names, types (e.g., copy only files starting with `fact`)

### ✅ ForEach Activity
- **Use Case**: Loop through each file and apply conditional logic to decide next steps

### ✅ Set Variable Activity
- **Use Case**: Assign a value to a variable during pipeline execution for dynamic control.

### ✅ Execute Pipeline Activity
- **Use Case**: Run a child pipeline from a parent pipeline to organize modular workflows.

### ✅ Data Flow Activity
- **Use Case**: Perform complex data transformations using a visual Spark-based interface.

### ✅ Delete Activity
- **Use Case**: Delete files or folders from supported storage locations as part of data cleanup.

### ✅ Wait Activity
- **Use Case**: Introduce a delay/pause in the pipeline execution. Useful in sequential processing or scheduling.

### ✅ Filter Activity
- **Use Case**: Filter an array of values in a pipeline. Often used with ForEach to process only specific items.

---

## 🧪 Real-Time Scenarios Covered
1. **Copy CSV from one container to another**
2. **Pull data from external HTTP (GitHub) and store in Data Lake**
3. **Conditionally copy only fact files to reporting container**
4. **Dynamic file naming and destination paths**
5. **File filtering using Get Metadata + If Condition + ForEach combo**

---

## ⏰ Triggers
### Schedule Trigger
- Run pipelines at specific times

### Tumbling Window Trigger
- Time-based, stateful pipeline executions

### Event-based Trigger
- Reacts to storage events like file arrival

---

## 🔐 Data Redundancy Models in Azure Storage
| Model | Description |
|-------|-------------|
| **LRS** | Locally redundant (3 copies in same region) |
| **ZRS** | Zone redundant (3 copies across zones) |
| **GRS** | Geo redundant (copies in different regions) |
| **GZRS** | Geo + Zone redundant (best durability) |

---

## 💻 Azure Portal Basics
- **portal.azure.com**
- **Resource Group**: Logical container for resources
- **Navigation**: Home > Resource Group > Resource (e.g., ADF or Storage)

---

## 🧰 Tools and Technologies Integrated
- Azure Data Factory
- Azure Data Lake Gen2
- GitHub (HTTP connector)
- CSV data files
- GUI-based development (no code transformations)

---

## ✅ Summary
By the end of this course, you’ve learned to:
- Build pipelines from scratch
- Connect to multiple data sources
- Migrate and transform data
- Use triggers and conditional logic
- Handle real-time business use cases

---

## 📎 Extra Resources
- [Ansh Lamba’s YouTube Channel](https://www.youtube.com/@AnshLambaJSR)
- [Azure Documentation](https://learn.microsoft.com/en-us/azure/data-factory/introduction)
- [GitHub Repo for Sample Data](https://github.com/anshlambagit)