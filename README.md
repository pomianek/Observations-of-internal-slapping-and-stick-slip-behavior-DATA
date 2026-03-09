# Four-Camera Stereo Digital Image Correlation Data for the Brake-Reuß Beam

Go to https://doi.org/10.5281/zenodo.18928738 to download files.

This repository contains the raw full-field measurement data from stereo digital image correlation (DIC) experiments on a Brake-Reuß beam with a bolted lap joint. The data were collected using two stereo camera pairs (four cameras total) and accompany the following publication:

> **Observations of internal slapping and stick-slip behavior in a bolted joint using 4-camera stereo DIC**
> Nicholas Pomianek, Trevor Jerome, Enrique Gutierrez-Wing, J. Gregory McDaniel
> Submitted to Mechanical Systems and Signal Processing, 2026. 

## Dataset Description

The raw DIC data are provided as MATLAB `.mat` files. Each file contains a cell array, where each element of the cell corresponds to a single stereo camera set. Within each cell element, the data are stored as a table with the following structure:

- **Rows** — each row corresponds to one DIC subset (i.e., one spatial measurement point)
- **Columns** — `x`, `y`, `z` columns correspond to absolute positions, displacements are the columns with the `displacement_` prefix. The point id column is an arbitrary subset id address that stays constant from one time step to another.
- **Force data** - the force data is stored as raw voltage and can be converted using:
force_cc = 22.13; % mV/N
force_cc = (1/force_cc)*1000; % N/V

- All data taken at 5000 Hz.

- Raw video data can be sent upon request.

- DIC analysis done using Zeiss Correlate 2025.

## Citation

If you use this data, please cite both the paper and the dataset:

**Paper:**
> [Full citation — to be added upon publication]

**Dataset:**
> [Author(s)]. ([Year]). *Four-Camera Stereo DIC Data for the Brake-Reuß Beam* [Data set]. Zenodo. https://doi.org/[zenodo-doi]

## License

This dataset is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the data for any purpose, provided you give appropriate credit.

## Contact

[Your Name] — [email address or ORCID link]
