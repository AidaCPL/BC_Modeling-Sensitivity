# CBA Equations for Nuclear District Heating

This README provides the core mathematical formulas used in our Cost-Benefit Analysis (CBA) model.  
They include:

- **Levelized Cost of Heat (LCOH)**
- **Net Present Value (NPV)**
- **Internal Rate of Return (IRR)**
- **Payback Period**
- **Marginal GHG Abatement Cost (MAC)**


---

```latex
\[
\textbf{Levelized Cost of Heat (LCOH):} 
\quad
\text{LCOH} 
= \frac{\text{Annual Cost}}{\text{Heat Demand}}
\]

\[
\text{where:} \quad
\text{Annual Cost} = \text{CAPEX} \times \text{Annuity Factor} + \text{OPEX}, 
\quad
\text{Annuity Factor} = \frac{r}{1 - (1 + r)^{-T}}
\]
\[
\text{(}r \text{ is the discount rate, and } T \text{ is the project lifetime.)}
\]

\[
\textbf{Net Present Value (NPV):}
\quad
\text{NPV}
= \sum_{t=1}^{T} 
\frac{\text{Revenue}_t - \text{OPEX}_t}{(1 + r)^t}
\;-\;
\text{CAPEX}
\]

\[
\textbf{Internal Rate of Return (IRR):}
\quad
0
= \sum_{t=1}^{T} 
\frac{\text{Revenue}_t - \text{OPEX}_t}{(1 + \text{IRR})^t}
\;-\;
\text{CAPEX}
\]
\[
\text{(IRR is the discount rate that sets NPV = 0.)}
\]

\[
\textbf{Payback Period (Simple Formula):}
\quad
\text{Payback Period}
= \frac{\text{CAPEX}}{\text{Annual Revenue} \;-\; \text{OPEX}}
\]

\[
\textbf{Marginal GHG Abatement Cost (MAC):}
\quad
\text{MAC}
= \frac{\text{LCOH} \times Q_{\text{DH}}}
{
\left(
E_{\text{BAU}} \times Q_{\text{DH}}
\right)
\;-\;
\left(
E_{\text{DH\_NCHP}} \times Q_{\text{DH}}
\right)
}
\]
\[
\text{where: } 
Q_{\text{DH}} \text{ is the annual district heat (MWh), }
E_{\text{BAU}} \text{ is the baseline emission factor (t CO}_2\text{/MWh), }
E_{\text{DH\_NCHP}} \text{ is the emission factor for nuclear district heating (t CO}_2\text{/MWh).}
\]

