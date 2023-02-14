Postgres
    No limits Scalable
    query processing
        buffer memory (work_mem)
            if buffer_memory is less, query processing spills on disk memory


portal azure
    monitoring
        metrics
            temp files > 0 (if temp files is being created, it means operation is happening in disk memory)
            disk iops

azure monitor
    metrics
    alerts

Logs
    log storage
    logz


Azure Postgres
    Single Server
    Flexible Server


Starting a Connection
    Forking on OS
    Memory Allocation

Connection Pooling
    can increase the tps by mananging connection efficiently
    postgres default port 6432
    sql server default port
    PGBouncer
        session
        transaction
        statement pooling

Flexible Server Architecture:
    chatty worload
        synchronous replication ? enable / disable

Local Disk Caching 
    Buffer pool extension
        unchanged pages

In Database,
     rows are stored in pages
     mysql/postgres - each has a pageblock size
