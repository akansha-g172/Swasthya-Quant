# Swasthya-Quant
HYBRID QUANTUM MACHINE LEARNING PROJECT - BENCHMARK EXPORT

Contents:
- models/: saved fitted model objects, if the objects were found and serializable
- graphs/: metric and runtime comparison graphs
- classical_reference.csv: supplied Logistic Regression, Classical SVM, Random Forest results
- four_feature_svm_qsvm.csv: direct four-feature SVM/QSVM results
- z_map_svm_qsvm.csv: supplied Z-map SVM/QSVM results including runtime
- qsvm_experiments.csv: feature-selection, PCA, ZZ and Z-map results
- svm_seed_stability.csv: classical SVM metrics for five seeds
- svm_stability_summary.csv: mean and sample standard deviation
- all_benchmark_tables.xlsx: all tables in separate worksheets
- model_save_status.csv: model serialization status

Interpretation:
1. Do not merge results from different experiments into one definitive ranking.
2. The original classical benchmark and the QSVM experiments may use different
   feature sets, splits, and configurations.
3. The four-feature SVM/QSVM table is the most relevant direct comparison
   among the supplied four-feature results, provided both rows used the same
   test split.
4. In the separate Z-map run, the classical SVM took 0.0217 seconds and the
   QSVM took 755.0195 seconds. Runtime is experiment-specific.
5. The QSVM confusion matrix is saved exactly as supplied.
6. This is an experimental research prototype, not a clinically validated
   diagnostic system.
