# subscription-data-platform
Built a batch data platform that moves subscription, payment, and device data through validation and cloud storage into a dimensional warehouse. Transforms the data into reporting marts for MRR, churn, and revenue analytics.

<img width="1205" height="361" alt="image" src="https://github.com/user-attachments/assets/7e1cc3d2-7fd6-466a-b9e5-9d6d4a69b7dc" />

**Receive source files:** Ingest the team’s subscription CSV batches from the designated S3 landing location.

**Validate the batch:** Check schemas, row counts, file metadata, and data quality before loading.

**Load to Snowflake:** Read the S3 files through a Snowflake stage and bulk-load them into RAW tables with COPY INTO.

**Transform with dbt:** Build staging views, core fact and dimension models, and reporting marts.

**Verify the outputs:** Run dbt data tests and capture customer-history snapshots.

**Enable analytics:** Use the marts to report on MRR, churn, subscriptions, and payment collections.
