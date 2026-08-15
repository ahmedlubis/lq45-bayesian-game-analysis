# LQ45 Bayesian Game Analysis

A financial market analysis that applies **Bayesian Game Theory** to study strategic behavior, information asymmetry, and trading decisions in Indonesia's LQ45 Index.

## 🎯 Problem

Financial markets involve participants with different levels of information, beliefs, and risk preferences.

This project asks:

* How do informed and uninformed traders differ in their payoff and risk profiles?
* How does actual trading behavior compare with the theoretically optimal strategy predicted by a **Bayesian Nash Equilibrium (BNE)**?
* Can Bayesian Game Theory help explain strategic behavior in an emerging stock market?

## 📊 Dataset

The analysis uses **daily observations of Indonesia's LQ45 Index**.

Key variables include:

| Variable   | Description                          |
| ---------- | ------------------------------------ |
| Price      | Adjusted closing price               |
| Volume     | Daily trading volume                 |
| Return     | Log return                           |
| Volatility | Rolling 10-day standard deviation    |
| RSI Lag    | 14-day RSI lagged by one trading day |

The dataset combines market price and volume information with technical indicators to construct empirical trading strategies.

## 🔬 Method

The analysis combines **financial data, technical indicators, and Bayesian Game Theory**.

### 1. Market Data Preparation

Daily LQ45 data are transformed into:

* Log returns
* Rolling volatility
* Lagged RSI
* Trading signals

### 2. Trader Types

The model distinguishes between:

**Informed traders**

Participants assumed to have better information or analytical advantages.

**Uninformed traders**

Participants who make decisions using publicly available market information and technical signals.

### 3. Payoff Modeling

Payoffs are constructed by incorporating:

* Trading returns
* Information premiums
* Risk penalties

This allows the payoff distributions of informed and uninformed traders to be compared.

### 4. Bayesian Game

A Bayesian Game framework is used to model strategic decisions under incomplete information.

The model estimates the **Bayesian Nash Equilibrium (BNE)** — the strategy combination in which each player chooses the optimal action given their beliefs about the other player's type.

### 5. Empirical vs. Theoretical Strategies

Actual market strategies are compared with the strategies predicted by the Bayesian Nash Equilibrium.

The available actions are:

`Buy` • `Hold` • `Sell`

## 📈 Results

### 1. Informed vs. Uninformed Payoffs

The payoff distributions show clear differences between the two trader types.

* Median payoffs for both groups are close to zero.
* Informed traders show substantially greater payoff dispersion.
* Their outcomes include both larger potential gains and larger potential losses.
* Uninformed traders have a narrower payoff distribution.

**Key insight:**

> Information advantage is associated with greater payoff variability rather than consistently higher returns.

This suggests that an information advantage can create greater opportunities while also increasing exposure to downside risk.

### 2. Actual Trading vs. Bayesian Nash Equilibrium

The empirical and theoretical strategy distributions differ substantially.

The observed market data show a strong preference for **Hold**, while the Bayesian Nash Equilibrium produces relatively more **Buy** and **Sell** decisions.

This suggests that actual market participants trade less frequently than the theoretical model would imply.

Possible explanations include:

* Transaction costs
* Market uncertainty
* Loss aversion
* Investor hesitation
* Behavioral factors
* Information not captured by the model

## 📊 Visualization

### Empirical Payoff Profile

![Empirical Payoff Profile](empirical_payoff_profile.png)

The distribution illustrates the difference in payoff variability between informed and uninformed trader types.

### Strategy Distribution: Actual vs. Bayesian Nash Equilibrium

![Strategy Distribution Comparison](strategy_distribution_comparison.png)

The comparison shows how observed trading behavior differs from the theoretically optimal Bayesian strategy.

## 💡 Conclusion

This analysis suggests three main findings:

1. **Information advantages come with higher payoff variability.**
   Informed traders have greater upside potential but also greater downside exposure.

2. **Actual trading behavior differs from theoretical equilibrium behavior.**
   Market participants show a stronger preference for holding positions than predicted by the Bayesian Nash Equilibrium.

3. **Bayesian Game Theory provides a useful benchmark, but not a complete explanation of market behavior.**
   Real-world decisions are influenced by behavioral factors, transaction costs, uncertainty, and other market frictions.

Overall, the project demonstrates how **game theory, financial data, and behavioral considerations** can be combined to study strategic decision-making in an emerging stock market.

## 🛠️ Technologies

* **R**
* **R Markdown**
* **Bayesian Game Theory**
* **Bayesian Nash Equilibrium**
* **Financial Data Analysis**
* **Statistical Analysis**
* **Technical Analysis**
* **Data Visualization**
* **Web Scraping**

## 📁 Repository Structure

```text
lq45-bayesian-game-analysis/
│
├── lq45-bayesian-game-analysis.Rmd
├── lq45-bayesian-game-analysis.md
├── empirical_payoff_profile.png
├── strategy_distribution_comparison.png
└── README.md
```

## 📌 Topics

`R` `Bayesian Game Theory` `Game Theory` `LQ45` `Financial Analysis` `Stock Market` `Bayesian Nash Equilibrium` `Behavioral Finance` `Data Analysis`
