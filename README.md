# Spring Batch

## What is Spring Batch?
- Spring Batch is an open source framework for batch processing
- Batch processing technique is process large of data in group instead of single element of data (use chunk method!)


## When To Use Spring Batch?

### Billing Analysis System
Use Case:
We have a lot of data in .csv file and we want to dump all the data inside database. It's take a long time if we want to put one by one right? So with batch processing it will be faster and automate dump data into database

- file.csv = source
- database = destination

### Report Generating System
Use Case:
We want to automate generating files everyday (schedule jobs)

- database (source)
- file.csv (destination)

## Architecture of Spring Batch

- Job launcher = The interface of spring batch used to launch jobs. (trigger job)
- Job = work which want to execute
- Job Repisotory = helps to maintain the jobs (status: success || failed) // state management
- Step: Represents a unit of work within a batch job.
- Chunk-Oriented Step: process data in chunks.
- Tasklet Step: execute a single task.

Reader: Retrieves data from a source, like a file or database.
Processor: Transforms or processes the input data.
Writer: Writes the processed data to a destination, like a file or database.

<footer>NaufalAzim 2024</footer>
