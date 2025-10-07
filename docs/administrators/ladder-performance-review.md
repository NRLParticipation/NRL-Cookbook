# Ladder performance review templates

**Category:** Administrators  
**Template type:** Interactive content creation

**Collect these inputs before you start:**

- [LEAGUE_NAME]
- [NUMBER_OF_DIVISIONS]
- [MISSION_STATEMENT]
- [ROUND_WINDOW]
- Latest MySideline ladder export details (file name, export date, divisions covered)


Analyse ladder reports for fairness across divisions. These prompts help competition administrators spot over- or under-performing teams quickly and recommend divisions that may need reshuffling.

---

## Low complexity: Ladder review prompt

Use this when you have a single MySideline ladder export and need a quick fairness scan with clear next steps.

```text
You are helping a competition administrator review the latest rugby league ladder export from MySideline to check if divisions are fair. Using the ladder report with divisions, teams, scores, points differential, and win/loss records, break the data down by division, calculate the division's average points differential, the standard deviation of points differential, and the win ratio range. Highlight standout teams and extreme underperformers. For every team you flag as a high anomaly, explain the specific metric (e.g., +218 points differential, 0% win ratio) that triggered the flag. Format each divisional summary exactly as shown below, replacing the placeholder values with the calculated metrics and observations:

Second Grade Men
Competitive Balance:
Average points difference: 47.1
Standard deviation: ~168
Win ratio range: 0 – 0.69
Melton Broncos, Eastern Raptors, and North West Wolves show strong performance
Standout Teams:
Melton Broncos – +218 PD, 69% win rate
Eastern Raptors – +148 PD, 63% win rate
North West Wolves – +174 PD, 63% win rate
Structural Risks:
Sunshine Cowboys: –432 PD, 0% win ratio → extreme outlier, urgent review
Multiple teams (Altona Roosters, Truganina Rabbitohs, Casey Warriors) slightly negative PD but competitive
Anomalies:
Sunshine Cowboys: High Concern (PD –432, 0% win ratio)
Doveton Steelers: Moderate Concern (PD +6, 62% win ratio)

After all divisional summaries, create a list of teams that should be checked to see if they should move up or down a division, including the anomaly reason for each team.
```

---

## Medium complexity: Ladder review workflow

Choose this option when you can provide the structured MySideline ladder export and need division-by-division recommendations ready for committee review.

```text
# NRL club workshop activity generator (medium complexity)

<ROLE_AND_GOAL>
You are a competition administrator tasked with analysing a rugby league ladder report to check fairness within each division and provide recommendations for divisional moves.
</ROLE_AND_GOAL>

<INPUT>
Provide the following information:
- **MySideline ladder export** including divisions, teams, scores, points differential, win/loss records, and export metadata (date, round range).
</INPUT>

<STEPS>
1. Break the ladder data down by division and calculate each division's average points differential, standard deviation, and win ratio range.
2. Identify teams that are consistently scoring significantly higher than their divisional peers and document the specific metric(s) that triggered the anomaly rating.
3. Highlight teams with unusually low performance and explain the contributing metric(s).
4. Format each divisional summary exactly as shown in the example below, replacing the placeholder values with the calculated metrics and observations:

Second Grade Men
Competitive Balance:
Average points difference: 47.1
Standard deviation: ~168
Win ratio range: 0 – 0.69
Melton Broncos, Eastern Raptors, and North West Wolves show strong performance
Standout Teams:
Melton Broncos – +218 PD, 69% win rate
Eastern Raptors – +148 PD, 63% win rate
North West Wolves – +174 PD, 63% win rate
Structural Risks:
Sunshine Cowboys: –432 PD, 0% win ratio → extreme outlier, urgent review
Multiple teams (Altona Roosters, Truganina Rabbitohs, Casey Warriors) slightly negative PD but competitive
Anomalies:
Sunshine Cowboys: High Concern (PD –432, 0% win ratio)
Doveton Steelers: Moderate Concern (PD +6, 62% win ratio)

5. Provide clear recommendations on whether any teams should be considered for moving up or down a division, referencing the calculated metrics from MySideline.
6. Create a final list of teams recommended for divisional review with the anomaly reason recorded for each.

<CONSTRAINTS>
- Base recommendations only on the data provided.
- Focus on fairness within each division.
- Keep the analysis short and actionable.
</CONSTRAINTS>

<OUTPUT>
- Division-by-division breakdown.
- Division-by-division sections mirroring the example structure: Competitive Balance (average PD, standard deviation, win ratio range, notable trends), Standout Teams (with metric callouts), Structural Risks (underperformers with metrics), and Anomalies (team + concern level + trigger metric).
- Clear recommendations on divisional changes with references to the MySideline export data points.
- Final list of teams to be assessed for possible moves, each annotated with the reason they were flagged.
```

---

## High complexity: Ladder equity audit orchestrator

Deploy this workflow when you need to reconcile multiple ladder reports, integrate match notes, and log evidence before proposing competition structure changes.

```text
# Ladder equity audit template (high complexity)

<ROLE_AND_GOAL>
You are the Competition Integrity Lead for [LEAGUE_NAME], conducting a full-season ladder equity audit across [NUMBER_OF_DIVISIONS] divisions using the MySideline ladder exports supplied. Your objective is to surface anomalies, recommend divisional moves, and flag governance actions while reinforcing [MISSION_STATEMENT].
</ROLE_AND_GOAL>

<SYSTEM_PARAMETERS>
- reasoning_effort: high
- tool_budget: 7 (statistical summaries, trend comparison, roster checks, anomaly detection)
- decision_mode: assess -> recommend -> verify
</SYSTEM_PARAMETERS>

<CONTEXT_GATHERING>
Goal: assemble the minimal data set needed for confident recommendations.
- Catalogue each MySideline ladder export (division, date range, format) and note any missing rounds.
- Capture team performance indicators (points for/against, win-loss streaks, points differential, bonus points) with source citations.
- Log contextual notes such as injuries, forfeits, or weather impacts when supplied.
- Flag divisions with inconsistent data and mark items for follow up.

<WORKFLOW>
1. Build a comparison table per division summarising ladder position, points differential, trend over the last [ROUND_WINDOW] rounds, average points differential, standard deviation, and win ratio range, referencing the MySideline export date/version.
2. Run anomaly checks for teams exceeding standard deviation thresholds or trailing the pack significantly; classify as high/medium/low concern and capture the specific statistic (e.g., points differential, win streak) that triggered the anomaly.
3. Draft narrative summaries for each division covering competitive balance, standout teams, and structural risks. Use the structure below as a guide for each division snapshot:

Second Grade Men
Competitive Balance:
Average points difference: 47.1
Standard deviation: ~168
Win ratio range: 0 – 0.69
Melton Broncos, Eastern Raptors, and North West Wolves show strong performance
Standout Teams:
Melton Broncos – +218 PD, 69% win rate
Eastern Raptors – +148 PD, 63% win rate
North West Wolves – +174 PD, 63% win rate
Structural Risks:
Sunshine Cowboys: –432 PD, 0% win ratio → extreme outlier, urgent review
Multiple teams (Altona Roosters, Truganina Rabbitohs, Casey Warriors) slightly negative PD but competitive
Anomalies:
Sunshine Cowboys: High Concern (PD –432, 0% win ratio)
Doveton Steelers: Moderate Concern (PD +6, 62% win ratio)

4. Recommend divisional moves or remedial actions (e.g., schedule adjustments, coaching support) with rationale and expected impact.
5. Create a governance-ready action register assigning owners, timelines, and evidence sources for every recommendation.
6. Suggest follow-up prompts or data requests required before final approval.

<VALIDATION>
- Confirm calculations for averages and differentials; list any assumptions made.
- Cross-check recommendations against league policies or promotion/relegation rules provided.
- Ensure every suggested move references supporting evidence in the context log.

<OUTPUT>
Produce a markdown briefing with:
### Division snapshots
- Bulleted summaries following the example structure (Competitive Balance metrics, Standout Teams with metric citations, Structural Risks, Anomalies with concern level and trigger statistic) using MySideline data.

### Recommendation register
- Table of proposed moves or interventions with justification, owner, timeline, and the anomaly reason drawn from MySideline data.

### Evidence appendix
- List of source documents (MySideline export names/dates), data extracts, and outstanding questions for leadership review.

### Next actions
- Ranked follow-up tasks (e.g., schedule review, club consultation) with suggested prompts.
```

---
