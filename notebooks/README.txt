1) High-risk counties cluster where both uninsured rates and poverty rates are simultaneously high, not just one or the other.  
2) Among the top-ranked counties, uninsured rates reach roughly the high 20s to 40%+, while poverty rates in the same counties can be ~25% to 50%+, indicating compounding access barriers.  
3) Using a rank-based composite score reduces the chance that one metric dominates (e.g., a county with extreme poverty but average uninsured, or vice versa), so the top 15 represent consistently high risk across both dimensions.  
4) This score should be treated as a screening tool: it identifies where access barriers may be highest, but it does not prove causality or measure actual clinic capacity.

LIMITATIONS
- County-level HIV metrics are suppressed in some counties due to small counts and privacy/statistical reliability. This analysis is therefore limited to counties with available prevalence estimates.

What you built: A county-level screening model combining HIV burden (prevalence rate) with access barriers (uninsured + poverty), plus viral suppression as an outcomes context metric.
How you scored: Percentile ranks for Need and Access, then a combined gap score (0–1).
Key result: A ranked list of counties with high burden + high barriers (top 15 table) and a national gap map.
Limitations: CDC suppresses some county values (small counts/privacy), so the gap score is computed only where prevalence is available.
Use case: Helps prioritize where to investigate capacity and outreach (not a causal claim).

