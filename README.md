# Airflow Tutorial
Airflow is a platform to programmatically author, schedule and monitor workflows.

# Setup
```bash
export AIRFLOW_GPL_UNIDECODE=yes

pip install -r requirements.txt
```

# Use cases
Batch processing jobs at set schedules for a large number of tasks. These jobs range from data analysis and metric aggregations, to brokerage operations such as dividend payouts.

[Robinhood's article](https://robinhood.engineering/why-robinhood-uses-airflow-aed13a9a90c8)

[Data transformation from multiple sources](https://medium.com/@dustinstansbury/understanding-apache-airflows-key-concepts-a96efed52b1a)

## Drawbacks of Cron Jobs
- poor job at handling task dependencies
- no strategy for retrying that task
- generates limited metadata about task landing times, execution durations, and failures of scheduled tasks
- simple management operations like inspecting and interacting with the CRON processes are difficult for any data stakeholder who lacks a system administration skill set.

## Alternatives to airflow
Google DataFlow for streaming data.

# References
https://airflow.apache.org/start.html