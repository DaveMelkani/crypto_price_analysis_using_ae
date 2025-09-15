# crypto_price_analysis_using_ae
implementing various AEs on large crypto dataset (with work on credit card dataset) to understand latent reps 
Data Preparation & Exploration
- Confirm dataset (crypto_df) consistency: token IDs, dates, and price metrics.
- Normalize or standardize features for autoencoder input.
- Perform initial exploratory analysis: distributions, correlations, missing data.

Model Implementation & Training
- Train Vanilla AE for basic reconstruction.
- Train Variational AE (VAE) for probabilistic latent embeddings.
- Train Denoising AE (DAE) to enhance robustness to noise.
- Train Conv1D AE for capturing sequential dependencies in crypto prices.
- Track training and validation losses, ensuring convergence.

Latent Space Analysis
- Extract latent embeddings (df_latents) for each model.
- Visualize embeddings using UMAP (emb_df) to detect clustering by token, sector, or temporal patterns.
- Compare latent spaces across different models for interpretability.

Reconstruction & Anomaly Detection

Compute reconstruction errors for all models.

Identify anomalies using thresholds (e.g., 95th percentile, 99th percentile).

Evaluate alignment between anomalies detected by different AE types.

Model Evaluation & Comparison

Quantitatively assess reconstruction performance (e.g., MSE, MAE).

Compare latent dimensionality reduction effectiveness.

Examine robustness to noise and temporal fluctuations.

Next Steps / Extensions

Hyperparameter Optimization: Grid or Bayesian search for latent dimension size, learning rate, and architecture depth.

Integration with Predictive Models: Use latent embeddings for downstream price prediction or portfolio risk analysis.

Anomaly Analysis: Investigate the economic or market significance of detected anomalies.

Report & Visualization: Create clear visual summaries comparing AE types, latent structures, and anomaly patterns.

Documentation: Ensure the notebook clearly shows workflow, methodology, and results to showcase proficiency in autoencoders.
