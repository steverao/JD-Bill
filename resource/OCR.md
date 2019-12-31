## Requirements

- To ensure the high reliability of the system, two sets of OCR recognition models from the big data department and the artificial intelligence department need to be simultaneously accessed.
- Provides manual control of the respective task ratios of the two models.
- During the running process, the recognition rate of the model can be calculated dynamically, and the task can be automatically divided according to the recognition rate.
- Have a cache regardless of the recognition result.
- Stores the recognition result information of all models in the database for analysis of the results of model running.



## Technology checklist

- Use OCR service through **RPC** service.
- Use **Redis** to cache bill recognition results, recognition rate of the models, etc.
- Asynchronous communication between systems using **Message Queue**.
- Use **Mysql** to store the Recognition result infomations of all models.
- Data persistence layer management with **mybatis**.
- Use **thread pool technology** to support high concurrency.