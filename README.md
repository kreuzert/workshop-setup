[![Jupyter4NFDI](https://nfdi-jupyter.de/docs/images/jupyter4nfdi_badge.svg)](https://hub.nfdi-jupyter.de/v2/gh/kreuzert/workshop-setup/main?labpath=%2Fhome%2Fjovyan%2Findex.ipynb)

# workshop-setup

Minimal [repo2docker](https://repo2docker.readthedocs.io/en/latest/) environment
for the **Generative AI Satellite Workshop** at the Helmholtz Imaging
Conference 2026 — [workshop website](https://scads.github.io/hic-genai-2026).

## Launch on Jupyter4NFDI

Click the badge above to build and start this environment on
[Jupyter4NFDI](https://nfdi-jupyter.de/docs/users/jupyterlab/repo2docker/).
`index.ipynb` is opened automatically via the URL-encoded `labpath` query
argument (`%2Fhome%2Fjovyan%2Fwork%2Findex.ipynb`).

## Data

The example data is downloaded from
[Zenodo](https://zenodo.org/records/24033766) during the image build by the
`postBuild` script and is available in `data/`:

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24033766.svg)](https://doi.org/10.5281/zenodo.24033766)

- `data/blobs.tif`
- `data/data.csv`
- `data/Haase_MRT_tfl3d1.tif`
- `data/membrane2d.tif`
- `data/timelapse.gif`
- `data/timelapse.tif`

## Environment

Python 3.12 conda environment `workshop` (see `environment.yml`) with pinned
package versions (latest as of 2026-11-27):

```console
pip install bia-bob==0.37.2 numpy==2.5.5 scipy==1.18.1 pandas==3.1.1 \
    scikit-learn==1.9.1 scikit-image==0.26.0 seaborn==0.13.2 \
    cellpose==4.2.1.1 stackview==0.19.1
```
