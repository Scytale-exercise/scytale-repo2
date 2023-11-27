# Scytale Home Assignment
Hi there!

In this home assignment, you'll be developing a Spark script to aggregate some data from PRs.

### Instructions
#### Extract
1. Get the all repository from Organization: Scytale-exercise (https://github.com/Scytale-exercise)
2. For each repository in the organization, Get all pull requests.
3. Save the data on JSON files.
#### Transform
**Please use Pyspark
1. Get the JSON files (from the extract phase) .
2. Transform the separate files into this table using Spark (Use schema).
3. Please save the data to a parquet file.


| Organization Name            | repository_id            | repository_name            | repository_owner                  | num_prs                               | num_prs_merged                               | merged_at                            | is_compliant                                                                |
|--------------------------|--------------------------|----------------------------|-----------------------------------|---------------------------------------|----------------------------------------------|--------------------------------------|-----------------------------------------------------------------------------|
| the first phase before '/' from field `full_name` from repositories | `raw.id` from repositories | `raw.name` from repositories | `raw.owner.login` from repositories | The number of PRs for each repository | The number of Merged PRs for each repository | The last date that a PR was merge in | (`num_prs` == `num_prs_merged`) AND (`repository_owner` contains "scytale") |

#### Notes
1. Not all repositories have a PR.
2. PRs merged != PRs closed

### Bonus
- Handle pagination.
- Handle rate limits.

### What we're looking for
- The code should work!
- Separation of concerns - good directory/file/logical structure.
- Readable code.
- Optimized Spark code.

---
Please send us a zip file/github repo with your solution when you finish.
If you have any questions please don't hesitate to reach us through email or the phone!

Enjoy!

-- *Scytale R&D*
