# MySQL plans and Config
These are the default plans and configuration options for MySQL across the supported cloud platforms (AWS, Azure and GCP.)

## Plans

| Plan | Version | CPUs | Memory Size | Disk Size |
|------|---------|------|-------------|-----------|
|Small | 3.7     | 2    | min 4GB     | 5GB       |
|Medium| 3.7     | 4    | min 8GB     | 10GB      |
|Large | 3.7     | 8    | min 16GB    | 20GB      |

## Configuration Options

| Option Name | Values | Default |
|-------------|--------|---------|
| version     | 3.6, 3.7| 3.7    |
| storage_gb  | 5 - 4096| 5      |

### Azure Notes
CPU/memory size mapped into [Azure sku's](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-vcore-resource-limits-single-databases) as follows:
| Plan  | Sku      |
|-------|----------|
| small | B_Gen5_2 |
| medium | GP_Gen5_4 |
| large | MO_Gen5_8 |

### AWS Notes
CPU/memory size mapped into [AWS instance types](https://aws.amazon.com/ec2/instance-types/) as follows:
| Plan  | Instance type |
|-------|----------|
| small | t3.medium |
| medium | t3.xlarge |
| large | t3a.2xlarge |

### GCP Notes
CPU/memory size mapped into [GCP tiers](https://cloud.google.com/sql/pricing#2nd-gen-pricing) as follows:
| Plan  | Tier     |
|-------|----------|
| small | db-n1-standard-2 |
| medium | db-n1-standard-4 |
| large | db-n1-standard-8 |
