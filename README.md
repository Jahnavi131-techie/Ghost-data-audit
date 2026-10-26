# Ghost Data Still Exists: Northstar Shop Deletion Audit Agent

An automated auditing agent built for the HackerRank Orchestrate challenge to detect residual user data across microservice databases post-deletion.

## Features
- **Data Auditing**: Validates 518 deletion requests from `requests.csv` across `account_service`, `security_service`, and `analytics_platform`.
- **Classification Engine**: Identifies compliant vs. non-compliant services, trace IDs, and reasons for residual records.
- **Trace Logging**: Formatted logging matching `AGENTS.md` specifications for transparent agent steering and reproducibility.

## Project Structure
- `main.py` / `gen.py`: Core logic for auditing and generating compliance datasets.
- `output.csv`: Complete audit results (518 records) mapping deletion statuses and verification chains.
- `log.txt`: Session traces and agent interaction logs.
- `code.zip`: Packaged challenge submission.

## How to Run
```bash
python main.py
