# agent-finder
Find nearby auto insurance agents using the Google Maps Places API, and dump them to a CSV file.

This script was written to help automate part of
my girlfriends job. Maybe someone else will find it useful too.

## Google Maps API Key
You must have the environment variable `GOOGLE_MAPS_API_KEY` set to a valid Google Maps API key.

In your shell configuration file (.zshrc, .bash_profile, .bashrc, etc):
```shell
export GOOGLE_MAPS_API_KEY=<your-api-key>
```

## Usage



Basic search:

```shell
python agent-finder.py "Los Angeles, CA"
```

You can also customize the CSV filename and the search radius (units = kilometers).
```shell
python agent-finder.py "Los Angeles, CA" --filename foo.csv --radius 50
```
