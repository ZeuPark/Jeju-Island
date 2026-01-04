# Jeju HVDC Analysis Report

**Analysis Period**: 2025-01-01 ~ 2025-09-30 (273 days)

---

## 1. Seasonal Patterns (Key Findings)

| Season | Avg Power (MW) | Reverse Flow Rate | Characteristics |
|--------|----------------|-------------------|-----------------|
| **Summer (Jul-Aug)** | 345 | 0% | Maximum demand due to cooling |
| **Spring (Apr-May)** | 164 | **38-40%** | Highest reverse flow, curtailment concentrated |
| **Winter (Jan-Mar)** | 226 | 6.6% | Stable due to heating demand |

### Monthly Details

| Month | Avg (MW) | Std Dev | Min | Max | Reverse Rate |
|-------|----------|---------|-----|-----|--------------|
| Jan | 249.0 | 75.9 | -69 | 377 | 1.7% |
| Feb | 214.2 | 84.1 | -84 | 380 | 6.0% |
| Mar | 215.5 | 88.1 | -59 | 369 | 12.2% |
| Apr | 150.5 | 111.4 | -171 | 350 | **39.9%** |
| May | 177.6 | 99.7 | -135 | 354 | **37.9%** |
| Jun | 205.8 | 86.4 | -149 | 443 | 25.6% |
| Jul | 317.5 | 85.0 | 122 | 535 | 0.0% |
| Aug | 372.5 | 72.6 | 166 | 557 | 0.0% |
| Sep | 336.2 | 80.4 | 96 | 534 | 0.2% |

---

## 2. Reverse Flow Analysis

### By HVDC Line

| Line | Capacity | Occurrence | Rate | Avg Power | Max Power |
|------|----------|------------|------|-----------|-----------|
| **HVDC#1** | 300 MW | 2,271 times | **34.7%** | -38.4 MW | -144.2 MW |
| HVDC#2 | 400 MW | 3 times | 0.0% | -0.0 MW | -0.0 MW |
| HVDC#3 | 200 MW | 425 times | 6.5% | -32.7 MW | -83.4 MW |

### By Hour (High Risk Hours: 13-15h with >20%)

| Hour | Reverse Rate | Risk Level |
|------|-------------|------------|
| 10h | 14.8% | Medium |
| 11h | 17.0% | Medium |
| 12h | 19.9% | Medium |
| **13h** | **21.5%** | High |
| **14h** | **22.7%** | High |
| **15h** | **20.9%** | High |
| 16h | 17.5% | Medium |

### Key Statistics
- **Days with reverse flow**: 57 days / 273 days (20.9%)
- **Severe reverse days** (6+ hours): 6 days

---

## 3. Hourly Patterns

| Time Period | Avg (MW) | Std Dev | Min | Max | Characteristics |
|-------------|----------|---------|-----|-----|-----------------|
| **Peak (18-22h)** | 310.1 | 99.6 | -49 | 557 | Evening demand maximum |
| Off-peak (23-9h) | 260.1 | 85.8 | -61 | 502 | Stable reception |
| **Light load (10-17h)** | 196.5 | 130.8 | -171 | 557 | Solar generation reduces demand |

### Peak Hour Distribution
- **Maximum power hours**: 20h (53 days), 19h (33 days), 21h (29 days)
- **Minimum power hours**: 13h (56 days), 14h (40 days), 12h (32 days)

---

## 4. Capacity Utilization

| Line | Capacity | Avg Util | Max Util | Notes |
|------|----------|----------|----------|-------|
| HVDC#1 | 300 MW | 12.3% | 46.8% | Mainly handles reverse flow |
| HVDC#2 | 400 MW | 40.5% | 74.2% | Primary power reception |
| **HVDC#3** | 200 MW | 25.3% | **88.8%** | Highest utilization |

---

## 5. Correlation Analysis

| Pair | Correlation | Interpretation |
|------|-------------|----------------|
| HVDC#2 - HVDC#3 | **0.602** | Strong positive - operated together |
| HVDC#1 - HVDC#3 | 0.331 | Moderate |
| HVDC#1 - HVDC#2 | 0.198 | Weak - independent operation |

---

## 6. Weekday Analysis

| Day | Avg (MW) | Std Dev | Reverse Rate |
|-----|----------|---------|--------------|
| Mon | 244.9 | 118.3 | 14.7% |
| Tue | 247.1 | 112.1 | 13.7% |
| Wed | 252.2 | 114.3 | 13.7% |
| Thu | 248.5 | 115.8 | 14.0% |
| Fri | 252.8 | 109.6 | 12.9% |
| Sat | 250.1 | 114.2 | 13.2% |
| Sun | 249.7 | 110.4 | 13.8% |

**Weekday vs Weekend**: No significant difference (249.1 MW vs 249.9 MW)

---

## 7. Key Insights

### Problem Areas
1. **Spring (Apr-May) curtailment concentration**: Increased solar/wind generation + decreased demand = surge in reverse flow
2. **Daytime (10-17h) challenge**: Solar peak coincides with low demand
3. **HVDC#1 handles reverse flow**: Most reverse flow goes through HVDC#1

### Positive Findings
1. **Summer stability**: No reverse flow due to cooling demand
2. **HVDC#3 high utilization**: Most efficiently used line (88.8% max)
3. **Strong HVDC#2-#3 coordination**: Correlation of 0.60 indicates coordinated operation

### Recommendations
1. Focus curtailment management on **April-May, 10-17h**
2. Consider ESS deployment for peak shaving during **13-15h**
3. Optimize HVDC#1 for bidirectional flow capacity
4. Explore demand response programs for spring low-demand periods

---

*Report generated: 2025*
