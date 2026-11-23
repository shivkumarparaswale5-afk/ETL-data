# ETL-data
end to end data pipeline for Full etl-process

from pathlib import Path

# Get project root directory
PROJECT_ROOT = Path(__file__).resolve().parent.parent

# Source data location
SOURCE_PATH = PROJECT_ROOT / "data" / "source" / "sales.csv"

# Lakehouse locations
LAKEHOUSE_PATH = PROJECT_ROOT / "data" / "lakehouse"

BRONZE_PATH = LAKEHOUSE_PATH / "bronze" / "sales"

SILVER_PATH = LAKEHOUSE_PATH / "silver" / "sales"

GOLD_PATH = LAKEHOUSE_PATH / "gold" / "sales_summary"

# Spark application name
APP_NAME = "EndToEndMedallionPipeline"

