# Reliable , Scalable and Maintainable Applications

Most ***Data Intensive applications*** are made from basic building blocks that solve some common functionality
1. Store data to be able to query/read them later ( Databases)
2. Remember the result of an expensive operation to speed up reads (Caches)
3. Allow uses to search data by keywords or filter ( Search Index )
4. Send data for processing asynchronously ( Stream processing )
5. Periodically crunch a large amount of accumulated data ( Batch processing) 


These tools share general similarity but differ because of their 
1. Data access patterns
2. Performance characteristics
and thus have very different implementations


| Term | Definition |
| ------- | ------------ |
|Reliability | The system should continue to work effectively even in case of adversity|
|Scalability | The system should be able to handle load without major degradation in performance |
|Maintainability | Upgrades and upkeep of the system can be done effectively and productively |


## Reliability 

A system is reliable if
1. Performs the functionality user expected
2. Can tolerate user errors
3. Performs under the expected volume and load
4. Prevents the system from unauthorized access or abuse

A system is considered reliable if it can tolerate faults. There are several kinds of faults
1. Hardware Fault
    Introducing redundancy for hardware or software redundancy for hardware ( RAID levels) is a good way to tackle this. 
    ** Additional Reading RAID levels
2. Software Fault or errors : Testing, monitoring, observability, record and restart to recover are some good ways to address these
3. Human Errors  : Some good ways to tackle this
    1. Clean API design or software system design makes it harder to make mistake
    2. Unit and Integration testing and testing throughout the whole development process
    3. Decouple the commonly made mistake so as to avoid human errors
    4. Provide sandbox to uncomplicate change and test in environments
    5. Introduce telemetry to capture stats and monitoring
    6. Proper training and management practices
    7. Allow easy recovery like configuration rollbacks
    
