Project Agents and Data Handling Rules

The following rules apply to all code and data work for this project

1. Data processing must start from the publisher original files only Do not read previously generated master tables or prior processed outputs
2. Original files are read only Do not modify delete relabel or overwrite original files
3. Before writing any parsing code inspect the actual JSON format the real field names and the set of unique raw labels
4. Do not guess field names or encodings from documentation Do not generate empty compatibility columns without a clear purpose
5. Manual damage labels must be strictly distinguished from publisher provided automatic prediction probabilities
6. Unlabeled damage must not be treated as healthy other damage or unknown as a training class
7. Record the source calculation rules and intended use for every derived field
8. For every filtering step report counts before and after and give exclusion reasons Do not silently drop data
9. Use relative paths or command line arguments Do not hardcode user specific filesystem paths in code
10. Use the minimal necessary dependencies Keep functions small focused and avoid duplicated code or unnecessary classes
11. At this stage implement only download structural checks image to label matching and class counts Do not run data processing or train models
12. Exclude raw data download archives virtual environments and any full local master table from git tracking
13. Code must contain only English language No non English outputs or comments are allowed in source files or generated artifacts
14. Code comments must not contain punctuation characters and must not include numeric ordered lists such as 1 2 3 or 1 2 3 with separators

Notes
- These rules are mandatory project policy and must be followed by all scripts notebooks and helpers
- Follow them strictly when you implement parsing matching and reporting steps
