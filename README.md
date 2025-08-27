# Cloud Data Pipeline with Dataflow & Terraform

An **automated** data pipeline built on **Google Dataflow** for processing, **Terraform** for infrastructure-as-code, and **Hugging Face** for data sourcing. This project will showcase how to ingest, transform, and deploy data workflows efficiently in the cloud.

## Key Features
- **Dataflow**: Real-time or batch data processing.
- **Terraform**: Infrastructure provisioning and management.

Ideal for **data engineers** and **ML practitioners** looking to build end-to-end cloud-native pipelines.

```
cloud-data-pipeline/
├── dataflow/                  # Dataflow jobs and processing logic
│   ├── jobs/                  # Individual job scripts (e.g., preprocessing.py)
│   ├── templates/             # Dataflow templates
│   ├── utils/                 # Shared utilities
│   └── tests/                 # Dataflow-specific tests
│
├── terraform/                 # Infrastructure as Code
│   ├── modules/               # Reusable Terraform modules
│   ├── main.tf                # Main configuration
│   ├── variables.tf           # Input variables
│   ├── outputs.tf             # Output values
│   └── backend.tf             # Remote state configuration
│
├── hf_data/                   # Hugging Face data integration
│   ├── scripts/               # Scripts to fetch/process datasets
│   ├── config/                # Dataset configurations
│   └── tests/                 # Data validation tests
│
├── config/                    # Global configurations
│   ├── pipeline_config.yaml   # Pipeline parameters
│   └── env_vars.env           # Environment variables (excluded via .gitignore)
│
├── tests/                     # Cross-component tests
│   ├── dataflow/              # Dataflow job tests
│   ├── terraform/             # Terraform compliance tests
│   └── integration/           # End-to-end tests
│
├── .github/
│   └── workflows/             # GitHub Actions CI/CD
│       ├── terraform.yml      # Terraform plan/apply workflow
│       ├── dataflow-tests.yml # Dataflow job tests
│       └── hf-data-tests.yml  # Hugging Face data validation
│
├── docs/
│   ├── setup.md               # Local/dev setup instructions
│   ├── architecture.md        # High-level design
│   └── ci-cd.md               # CI/CD workflow details
│
├── scripts/                   # Utility scripts
│
├── .gitignore                 # Ignore secrets, logs, and local env files
├── README.md                  # Project overview, setup, and usage
├── requirements.txt           # Python dependencies
└── requirements-dev.txt       # Dev/test dependencies
```
