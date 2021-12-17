## Building the website

1. Create conda environment.
   ```
   conda env create -f zebrafishtfm-website.yml
   ```
2. Activate conda environment.
   ```
   conda activate zebrafishtfm-website
   ```
3. Serve website locally.
   ```
   mkdocs serve
   ```
4. Publish new website on github
   ```
   mkdocs gh-deploy
   ```
