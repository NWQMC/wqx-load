# wqx-load

Download and restore into database EPA WQX Water Quality Data.

## Overview
This repository contains scripts and a Jenkins pipeline to download Postgres wqx dump files from the
epa and load them into the wqx_dump schema in the observations database. This data is subsequently
transformed and loaded into the Water Quailty Portal database by the epa etl.

#### Environment variable definitions
See header comments in load_epa_wqx_dump_files.sh for environment variables required. The download script
epa_wqx_download.py does not use any environment variables.
