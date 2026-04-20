This work develops a framework model implemented in Python to support the
selection of option strategies on short-term interest rate (STIR) futures starting
from a qualitative market view.
The framework translates a market scenario into quantitative assumptions,
generates a realistic universe of finite-risk option structures, and evaluates them
using PnL-based metrics. Rather than focusing on a single trade, the frame
work is designed to highlight dominant strategies and explicit trade-offs across
risk, payoff shape, time decay, and maturity.
The Python model constructs option strategy universes, prices all option
legs using a Black-76 framework with transparent volatility assumptions,
evaluates strategies in terms of realized PnL rather than raw payoff, incorpo
rates time and maturity effects through theta proxies and roll comparisons, and
ranks strategies using scenario-dependent criteria reflecting the underlying mar
ket view. Exact market calibration is not pursued, as the focus of the task is on
reasoning and structure rather than precise valuation. Discounting effects are
treated in a simplified manner given the short maturities involved.
The framework is applied to two distinct cases. In the EURIBOR case, a
range-bound, short-volatility environment is considered, and the model favors
strategies combining robustness around the landing zone, premium dynamics,
and favorable roll characteristics. In the SONIA case, a directional scenario
associated with a potential rate cut is analyzed, shifting the focus toward delta
and gamma efficiency, convexity, and explicit maturity comparison between X5
and Z5.
Graphical outputs, such as PnL-at-expiry profiles and cross-maturity value
comparisons, are used to validate and interpret the model results, ensuring
that selected strategies are not only quantitatively ranked but also intuitively
understandable.
Overall, the main contribution of this work is the construction of a re
producible decision framework that replaces manual strike scanning with
an automated process. The selected strategies are presented as examples of
model output, illustrating how the framework supports consistent and informed
decision-making while leaving final judgment and execution to the trader or
broker.
