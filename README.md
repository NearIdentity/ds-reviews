# Review of Data Science Concepts

Jupyter Notebooks for reviewing Data Science (DS) concepts 

## Jupyter Notebook Format

* Conceptual Review
* Listing of potentially relevant Python libraries
* References
* Python-based examples

## Listing of Topics Covered

1. Mitigation of Extreme Class Imbalance (in Binary Classifiers)
2. Dual-Model Architecture
3. Partial Pooling
4. Hierarchical Priors
5. Cold-Start Behaviour
6. Drift Detection & Mitigation

## Installation & Use


### Installation

Recommended Python version: 3.12.x

```bash
bash ./venv-setup.sh -b python3.12 -d $PWD/
source ./venv/bin/activate
python3 -m pip install -r ./requirements.txt
```

### Jupyter Notebook Execution

```bash
source ./venv/bin/activate
jupyter-notebook ./ipynb/<notebook_filename>
```

## References & Additional Resources

### Foundational References

* Gelman, A., et al. (2013). _Bayesian Data Analysis_ (3rd ed.). Chapman and Hall/CRC.
* Hastie, T., Tibshirani, R., & Friedman, J. (2009). _The Elements of Statistical Learning_ (2nd ed.). Springer.
* Bishop, C. M. (2006). _Pattern Recognition and Machine Learning_. Springer.

### Imbalanced Classification

* Chawla, N. V., et al. (2002). "SMOTE: Synthetic Minority Over-sampling Technique." _JAIR_, **16**, 321-357.
* He, H., & Garcia, E. A. (2009). "Learning from Imbalanced Data." _IEEE TKDE_, **21**(9), 1263-1284.

### Mixture of Experts & Gating

* Jacobs, R. A., et al. (1991). "Adaptive Mixtures of Local Experts." _Neural Computation_, **3**(1), 79-87.
* Shazeer, N., et al. (2017). "Outrageously Large Neural Networks for Efficient Conditional Computation." _ICLR_.

### Partial Pooling & Hierarchical Priors

* Efron, B., & Morris, C. (1977). "Stein's Estimation Rule and Its Competitors." _JASA_, **68**(341), 117-130.
* Kruschke, J. K. (2014). _Doing Bayesian Data Analysis_. Academic Press.

### Drift Detection

* Gama, J., et al. (2014). "Learning from Streaming Data." _JMLR_, **15**, 49-76.
* Kuncheva, L. I. (2008). "Classifier Ensemble for Changing Environments." _Proceedings of ECDL_, 1-10.

## Appendix: Quick Reference — Which Technique When?

| Problem | Recommended Techniques | Key Libraries |
| :--- | :--- | :--- |
| Rare event prediction | SMOTE, cost weighting, threshold tuning | `imbalanced-learn`, `xgboost` |
| Multi-tier decisions | Dual-model, mixture of experts | `scikit-learn`, `tensorflow`  |
| Limited labeled data | Transfer learning, few-shot learning | `pytorch`, `tensorflow` |
| Group-level variation | Partial pooling, hierarchical models | `pymc`, `bambi` |
| New entities, sparse history | Content-based features, warm-starting | `scikit-learn`, `modAL` |
| Model degradation | Drift detection, online learning, retraining | `river`, `alibi-detect`, `evidently` |


