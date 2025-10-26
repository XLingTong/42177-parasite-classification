Large image data are not stored in GitHub.

To reproduce locally:

1. Download the raw Mendeley Parasite Dataset (v3):
   https://doi.org/10.17632/38jtn4nzs6.3

2. Place it under:
   for example: D:\LocalUser\42177 Project\raw\

3. Run src/preprocess/preprocess_pipeline_rgb.mlx
   to generate:
     data/clean/     → normalized 256×256 images
     data/degraded/  → degraded robustness sets

| Dataset size  | Typical I/O speed (SSD) | Estimated total runtime |
| ------------- | ----------------------- | ----------------------- |
| 5 000 images  | 300–400 MB/s            | 2–3 minutes             |
| 10 000 images | 300–400 MB/s            | 4–6 minutes             |
| 30 000 images | 300–400 MB/s            | 10–15 minutes           |
| 50 000 images | 300–400 MB/s            | 15–25 minutes           |

4. Use data/manifest.csv for labels and subsets.
