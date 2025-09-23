# Data ingestion

## Data ingestion

* Data Ingestion is the process of gathering, managing, and utilizing data efficiently.
* plays a foundational step in the data processing pipeline.
* It involves the seamless importation, transfer, or loading of raw data from diverse external source into centalized system where it awaits further processing and analysis.

## key steps in the ingestion process 

* Data collection : Gather raw data from various sources.
* Data transformation : clean,normalise , enrich the data.
* Data loading : move the transformed data into the target system.

## Types

* Batch
* Real time
* Micro-batching

<img width="1072" height="583" alt="image" src="https://github.com/user-attachments/assets/ca9d027a-7c52-447f-86a2-fde4eb0cacf0" />



## The Data ingestion workflow

* Data source identification : identify and register the data sources. Understand data fomal, structure, and access method.
* Data Extraction : Extract data from identified sources using connectors,APIs or other methods., Ensure the data is collected efficiantly and securely.
* Data Staging: Store the raw data in a staging area temporarily. This allows for initial checks and validation before transformation.
* Data Validation: Validate the collected data for accuracy and completeness. Identify and address any anomalles or errors at this stage.
* Data Transformation: Perform necessary transformations, including cleaning, normalization, and enrichment, to prepare the data for loading.
* Data Loading: Load the transformed data into the target storage or processing system. Ensure the data is Indexed, partitioned, and stored optimally.
* Data Monitoring: Continuously monitor performance, detect issues, and make necessary adjustments.

## Batch processing

* Technique where data is collected, store over the period of time.
* Processed together as a single unit or batch instead of being processed immediately.

* Data collection : Data from various sources is collected.
* Batch formation : The data is grouped in to batches based on time or size.
* Processing : A batch job or pipeline process the entire batch at once.
* Output or storage : processed results are stored in a database, file, or sent to other system for further use.

## Characteristics

* Latency : High. Not suitable for immediate use.
* Data size : Handles large volumes efficiantly.
* Processing : Done in groups, not per individual records.
* Scheduling : Usually triggered by time or event based triggers.
* Fault Tolerance : Easier to retryl restart failed batches.
* Cost : Generally cheaper than real-time processing for large volumes.

## Advantages

* Efficiency at scale : Process large volumes of data all at once, which is often more resource-efficient than handling each task individually.
* Automated scheduling : ideal for tasks that dont need real time results. it can run over night or during off peak hours.
* Error Handling and retry logic : Easier to apply consistent error handling, rollback mechanisms, or validation across the batch, which improves realibility.
* Reduced manual intervensions : once setup batch jobs can run automatically, minimizing human involvement and freeing up time for other tasks.
* Resourse optimizations : Because data is processed inbulk, it's often more CPU and memory efficient, especially when operations are predictable.
* Consistency and standardization : Ideal for applying the same transformation or logic across a dataset, which supports data consistency across the board.

## Limitations Of Batch processing 

* Delayed results
* Resource spikes
* Complex debugging
* Limited fluxibility
* Data staleness

## Batch processing architecture

![fedc67de-101f-4272-a7e0-f8cc5b884d3c](https://github.com/user-attachments/assets/d3b01558-8e4d-4fd2-8639-38933ceaa9cd)

## Common batch processing tools

* Apache Spark (batch mode)
* Apache Hadoop
* Talend
* AWS Glue
* Google Dataflow (batch mode)
* Asure Data factory

## Steam processing
* Continuous and real time processing of data as it flows in one record or event at a time there is no delay between data arrival and processing.
* Data ingestion : Data is continuously ingested from sources like Kafka, sensors, logs, APIs.
* Real time processing : Each event is processed as it arrives (e.g., filtering, aggregating, joining).
* Delivery : Results are pushed immediately to databases, dashboards, alerting systems, or APIs.


## Characteristics

* Feature : Description.
* Latency : Very low - near real time.
* Data size : Designed for ongoing, unbounded streams of data.
* Processing : Pre record or small time windows.
* Use case : Real time insights, monitoring, alerting.
* Fault Tolerance : Manage via checkpoints and windowing.
* Cost : More compute- intensive, potentially higher cost.

## Examples

* Fraud detection in banking
* real time ride matching (uber,ola)
* real time analytics for ecommerce
* social media feeds and notifications
* log monitoring and alerting
* online gaming leader boards
* stock marlet data and alerts
* video live streaming analytics
* smart traffic systems

## Advantages

* Data handled as a continuous, unbounded flow.
* Processing is real-time; insights delivered instantly.
* Essential for instant decision-making, such as real-time recommendations.
* Demands high-availability, always-on infrastructure.
* Errors and anomalies detected as they occur, enabling immediate action.


## Sream processing architecture


![0794fad8-e585-4ea3-826b-6491481e4680](https://github.com/user-attachments/assets/1ceac3a0-2b17-477b-8a8c-40f3ed86f869)

![0d03b13a-519e-4965-a2c6-88cddc9b9745](https://github.com/user-attachments/assets/62464f42-0389-44d7-a2b9-ed3f94d03618)
