<img width="4500" height="1200" alt="individual_level_scientific_fixed (1)" src="https://github.com/user-attachments/assets/2a617e4b-951c-4a32-ac18-1a168bd3d41f" />
Figure 1: Simulation Results I – Individual Algorithmic Nudging. 
Simulation of the bounded-confidence Bayesian updating mechanics at the individual user level. The user update rule (assuming an update rate of α = 1) is governed by: ωkt+1 = ωkt + (gm - ωkt) × exp(-κ(gm - ωkt)2).
Panel A (The Perfect Echo): Prior = 0.5, Signal = 0.5. Because the Distance is 0.0, the exponential penalty is zero. Beliefs remain perfectly static at 0.5.
Panel B (The Algorithmic Nudge): The Deep Q-Network learns to serve content just inside the confidence bound to maximize engagement. With a Prior of 0.5 and Signal of 0.7 (Distance = 0.2), the Confirmation Gate stays 88% open, successfully dragging the user's belief to 0.68.
Panel C (The Rejection Penalty): Prior = 0.5, Signal = -0.5 (Distance = 1.0). The Confirmation Bias Gate slams shut at exp(-3) ≈ 0.05. The user rejects the content, shifting negligibly to 0.45, causing engagement to flatline.
<img width="4500" height="1200" alt="population_level_fixed (1)" src="https://github.com/user-attachments/assets/798760ab-0c7f-4c76-af60-d883aa8b8c67" />
Figure 2: Simulation Results II – Population Polarization & Regulatory Policy. Monte Carlo simulation of the Human-AI Markov Game (N = 1,000 agents, t = 100 periods). The AI maximizes a weighted utility function balancing direct user engagement against a regulatory diversity constraint (γ): Uplatform = Engagement(gm, ωkt) + γ × Diversity(gm).Panel A (Baseline): Establishes the initial normally distributed prior belief state at Time t = 0. Panel B (Unregulated Filter Bubbles): Without a diversity mandate (γ = 0), the AI autonomously induces extreme informational segregation to optimize engagement, completely hollowing out the moderate center into isolated, bimodal echo chambers. Panel C (Regulatory Intervention): Activating the diversity constraint (γ > 0) forces the AI to cross-pollinate content. This penalty on slate homogeneity effectively pierces the filter bubble, neutralizing ideological drift and preserving the baseline societal distribution.
<img width="4500" height="1200" alt="kappa_sensitivity_scientific (1)" src="https://github.com/user-attachments/assets/ed411b06-4be0-44c8-9297-8bd80b7c7fbb" />
Figure 3: Robustness Check – Sensitivity to Confirmation Bias (κ).
Sensitivity analysis of the belief updating equation holding algorithmic distance constant (|gm - ωkt| = 0.2).
Low κ (Open-Minded): The exponential penalty is weak. The AI can rapidly drag the user's belief almost entirely toward the signal (ω → 0.7).
Baseline κ (Moderate): The AI successfully executes the standard incremental nudge (ω → 0.68).
High κ (Hyper-Partisan): The bounded confidence threshold is too narrow. Even a tiny nudge of 0.2 triggers total rejection (ω stays at 0.5). Conclusion: To maintain engagement with stubborn users, the AI is mathematically forced to abandon nudging and trap them in static Filter Bubbles.


# IO-of-AI-Project
algorithmic-market-failures
