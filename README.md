**Value at Risk (VaR)**

VaR is a Risk management Monitoring tool to asses the expected potential loss in value of an asset or portfolio at given
1. Specific time period
2. Confidence level

###**why VaR is calculated ?**
  
  VaR is calulated to Set Trading Limits, adjust Positions and to maintain Regulatory compliance


###**Methods**

1.   Historical Method
2.   Parametric Method
3.   Monte - Carlo Simulations Method


###**Limitations of VaR**
1. Does not indidcates the actual magnitude of losses
2. If the CI goes up the VaR goes up
3. Holding period goes up , VaR goes up
4. It fails to asses the Tail Risk.
5. Model Risk and Implementing risk

---
---

###**Data Collection**
 For this project Stock prices were derived from yahoo finance.

 Returns - Returns were calculated as log normal returns because normal return are not

 Portfolio weights remain constant

---
---

###**1. Historical Method**

**Assumption**

The Historical Simulation method calculates VaR by revaluing today’s portfolio using actual past market movements and taking the empirical percentile of the loss distribution. It avoids distributional assumptions and captures nonlinearities, but it is backward-looking and sensitive to the historical window selection.

**Model Assumptions**

1. Depends on the past price data, The History repeats itself
2. No assumptions on return distributipns. Doesn't follow random normal distribution,Does not assume symmetric distribution
3. Non - Parametric
4. Returns are stationary
5. Correlations remain stable, No need to estimate volatility/correlation parameters
6. Liquidity remains unchanged

**Advantages**
1. Since No distribution assumption, it Works better for options and nonlinear portfolios.

**Limitations**

1. Captures fat tails but fails to quantify the Extreme losses.
2. HS-VaR fails because it assumes the future will resemble the past, which breaks down when volatility, correlations, or market microstructure change abruptly.
During regime shifts (e.g., COVID, GFC, rate-hike cycles):

    *   Volatility jumps suddenly
    *   Correlations converge toward 1
    *   Liquidity risk

3. Historical window length affects the VaR - Sensitive to Sample size. Usually converges to larger sample.
    * Short windows → noisy VaR and frequent limit breaches, Volatile, Recent shocks
    * Long windows → Stable return distributions, but poor stress awareness and less relevant 

---
---
