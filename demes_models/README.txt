The directory `model_fits` contains our reported best fit models for the
different parameterizations.

Models are given in Demes format (Gower et al., 2022; doi:
https://doi.org/10.1101/2022.05.31.494112). The `description` field in the
YAML-formatted models also gives the log-likelihood for that fit.

The directory `validation_fits` contains re-evaluations of our best-fit models
from two scenarios, the continuous migration model and the multiple merger
model (each with migration between stem populations). These refit models
correspond to the supplementary results (Section S7), and are organized into
sub-directories for each validation scenario, keyed by the Supporting
Information section.

The directory `validation_models` contains fits corresponding to section S7, as
follows:

S7.1: Model fits using alternative datasets

- YRI_CEU: Fits replacing MSL with YRI and GBR with CEU.
- TSI: Fits replacing GBR with TSI.
- Nama_map: Fits using statistics computed from a Nama-specific recombination
  map.
- Nama_thresholds: Fits using a subset of Nama individuals, based on minimum
  estimated ancestry proportions (90% and 99%).

S7.2: Relaxed inference of divergence times

- deeper_fixed_divergences: Fits with the OOA event fixed at 60ka instead of
  50ka, and the E/W African split fixed at 100ka instead of 60ka.
- relaxed_divergences: Fits allowing the OOA and E/W African split times to be
  fit.

S7.8: Allowing for additional migrations

- additional_migrations: Fits with continuous symmetric migration between Mende
  and Nama, and between British and Nama, which have lower rates than between
  other pairs of populations.

S7.9: Replacing the reference population for statistics normalization

- Gumuz_normalization: Fits with statistics normalized using pairwise diversity
  and two-locus heterozygosity in the Gumuz, instead of Mende.
