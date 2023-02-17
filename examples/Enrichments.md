# Using Enrichments Python

Using enrichments with [Outscraper API](https://app.outscraper.com/api-docs#tag/Google-Maps).

## Installation

Python 3+
```bash
pip install outscraper
```

[Link to the Python package page](https://pypi.org/project/outscraper/)

## Initialization
```python
from outscraper import ApiClient

client = ApiClient(api_key='SECRET_API_KEY')
```
[Link to the profile page to create the API key](https://app.outscraper.com/profile)

## Usage

```python
# Enriching data from Google Maps with Emails & Contacts Scraper (domains_service) and validating emails with Email Validator (emails_validator_service):
results = client.google_maps_search('bars ny usa', enrichment=['domains_service', 'emails_validator_service'])
```