FOUND: The placebo simulation's random seed was left blank ("seed ____"), which would let a
researcher try multiple seeds and report whichever placebo distribution made the strategy
look strongest.
FIX: Locked the seed: numpy default_rng(seed=4075).

FOUND: "Percentile in the placebo distribution of gaps" did not specify exactly how the
percentile would be calculated.
FIX: Added "percentile = 100 × (# placebo gaps <= strategy gap) / 1000."
