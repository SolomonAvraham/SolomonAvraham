# DCA Tracker Setup Guide

## INVESTMENT SUMMARY DASHBOARD:
- **Total Amount Invested:**  =SUM('DCA Summary'!D:D)
- **Total Fees Paid:**  =SUM('DCA Summary'!G:G)
- **Total Net Cost:**  =Total Invested + Total Fees
- **Current Portfolio Value:**  =SUM('DCA Summary'!J:J)
- **Total Profit/Loss:**  =Current Value - Net Cost
- **Overall P/L %:**  =(Total P/L / Net Cost) × 100

---

## Sheet 1: DCA SUMMARY
| Column | Description |
|---|---|
| A | **Date** (Date format) |
| B | **Exchange** (Text - Bit2C) |
| C | **Currency Pair** (Text - BTC/ILS, ETH/ILS) |
| D | **Amount Invested (₪)** (Number) |
| E | **Crypto Purchased** (Number) |
| F | **Price per Unit**  = D/E |
| G | **Fees (₪)** (Number) |
| H | **Net Cost** = D+G |
| I | **Current Price (₪)** (Manual) |
| J | **Current Value** = E×I |
| K | **Profit/Loss** = J-H |
| L | **P/L %** = (K/H)×100 |

---

## Sheet 2: PORTFOLIO OVERVIEW
- **Total Amount Held:** =SUMIF(...)
- **Average Purchase Price:** (To be defined)
- **Total Invested:** (To be defined)
- **Total Fees:** (To be defined)
- **Current Value:** (To be defined)
- **Profit/Loss:** (To be defined)
- **P/L %:** (To be defined)
- **Portfolio Weight %:** (To be defined)

---

## Sheet 3: MONTHLY SUMMARY
(Monthly aggregations to be defined)

---

## Conditional Formatting Instructions:
- **Green for Profit:** Set rule to highlight cells in green where Profit/Loss (Column K) > 0.
- **Red for Loss:** Set rule to highlight cells in red where Profit/Loss (Column K) < 0.

---

## Usage Instructions:
1. Enter your investment details in the **DCA SUMMARY** sheet.
2. Update the **Current Price** in Column I regularly to reflect market conditions.
3. Review the **INVESTMENT SUMMARY DASHBOARD** for overall performance.
4. Use the **PORTFOLIO OVERVIEW** sheet to analyze your holdings by cryptocurrency.
5. Track your monthly performance in the **MONTHLY SUMMARY** sheet.