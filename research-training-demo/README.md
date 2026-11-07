# Research-methods teaching example: from social media data to networks

A **draft educational demonstration** for arts, humanities and social science researchers.

**Scope:** synthetic data only. Uses Python/pandas to clean a prepared social-media-style CSV, calculate engagement and activity, and produce a directed weighted edge list suitable for importing into Gephi. It does **not** collect live social-media data, involve an API, or use any material from Dr Eva Ferron's doctoral research.

This is a separate public branch of the existing TwiXplorer fork. **It is not part of TwiXplorer** and does not alter the original software. A dedicated repository would be preferable for long-term use.

## Run the example

Requires Python 3.10+.

```bash
python -m pip install -r requirements.txt
python activity_to_network.py
```

Expected output: 12 synthetic posts, 10 unique directed edges, and files under `outputs/`:
- `activity_by_day.csv`
- `engagement_by_author.csv`
- `gephi_edges.csv`
- `activity_by_day.png`

## Guided workshop activity

1. Inspect `data/synthetic_posts.csv`, identifying actors, mentions, timestamps and engagement.
2. Run the script and inspect its validation, grouping and output steps.
3. Import `outputs/gephi_edges.csv` into Gephi as an **edges table**, specifying a directed graph.
4. Compare indegree and weighted indegree. Neither measure alone establishes political influence.
5. Change a fictional mention in the source data, run the script again and explain the changed results.

## Limitations and next steps

This introductory draft has been script-tested using its synthetic dataset; current-version Gephi import and live classroom usability have **not** yet been independently validated. Before use as institutional training, check reproducibility in a clean environment, accessibility, licensing and feedback from learners.

**Attribution:** This example was prepared with AI assistance for Dr Eva Ferron's review and adaptation, and should not be represented as a previously delivered or peer-reviewed training course.

No institutional endorsement is claimed.

## Author and academic context

Dr Eva Ferron researches digital politics, social network analysis and computational text analysis (including word frequencies, keyness, collocations and KWIC). [ORCID](https://orcid.org/0000-0002-2269-7991).
