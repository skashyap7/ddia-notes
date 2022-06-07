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
