# Clash Royale Deck Composition & Match Outcome Prediction

This project explores whether **Clash Royale deck composition** can predict battle outcomes after reducing the effects of **skill disparity** and **card-level imbalance**.

Using battle logs from the official Clash Royale API, together with external card metadata and troop statistics, the project engineers deck-level features such as archetype counts, average elixir, combat-physics variables, matchup deltas, synergy indicators, and one-hot card representations.

Three models were tested: **XGBoost**, **Random Forest**, and **MLP**.  
The best result came from **XGBoost**, which achieved **58.21% testing accuracy**, slightly above the project’s **57.1% Elo-style benchmark**.

The findings suggest that deck composition contains **meaningful but moderate predictive signal**, while match outcomes still depend heavily on in-battle execution and other unobserved factors.
