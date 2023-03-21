
# flex-platform-services-metadata
<p align="center">
<img src="https://badge.buildkite.com/91fd09cef739378d54cd62ed4ec8cff35065805fa8459d7a10.svg">
<img src="https://img.shields.io/badge/python-v3.10-green">
<img src="https://img.shields.io/badge/code%20style-black-green.svg">
<img src="https://img.shields.io/badge/yaml%20config-yamllint-green">
</p>

This is a API service which provides metadata of services or roles managed by Flex Platform Team.

## Repository Structure

Please create a new config file in `data` directory, 
we follow file name as `data/<bu_name>/<service_name>/data.yaml`

Utilities to create and update configs in bulk are in future roadmap, for now you can use `data/flex/flex-buildkite-agent/data.yaml` as starting point.
Refer `api/schema.py` for pydantic schema definitions for allowed metadata fields

## Developer setup

1. Setup python 3.10 and above
2. Setup virtualenv `virtualenv -p python3 venv; source venv/bin/activate`
3. Setup dependencies with pip `pip install -r requirements.txt`
4. Run locally with `make local`
5. Refer `Makefile` for other helpful make goals

Browse below links to explore on local
1. http://localhost:8000/docs
2. http://localhost:8000/redoc
3. http://localhost:8000/health
4. http://localhost:8000/services
5. http://localhost:8000/services/flex-buildkite-agent
