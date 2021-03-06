## 0.0.12 - 07/27/2020
- Fix issue where packages with CLI functionality were not available on path

Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.12`

## 0.0.11 - 06/15/2020
- Add terra-notebook-utils to base image
- Add /home/jupyter-user/notebooks/packages to PYTHONPATH so user package installs persist using PDs

Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.11`

## 0.0.10 - 05/18/2020
- Adds jupyter notebook extension collapsible headers and code-folding

Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.10`

## 0.0.9 - 02/25/2020
- Fixes https://broadworkbench.atlassian.net/browse/IA-1676 in `google_sign_in.js` 
    - Adds a fallback method to set needed config when in non-notebook views
- Lints .js files
- Fixes bug in `edit-mode.js` that caused errors in console due to modules loading prematurely
    - also renames saveAs function due to global namespace conflicts with https://github.com/eligrey/FileSaver.js
   
Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.9`

## 0.0.8 - 02/05/2020

- Fix bug in `google_sign_in.js` in the base image
   - See https://broadworkbench.atlassian.net/browse/IA-1653

Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.8`

## 0.0.7 - 01/17/2020

- Make image locally runnable with:
   - `docker run --rm -it -p 8000:8000 <image>`
- Add FISS to base image
- Add OpenJDK 11 to base image

Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.7`

## 0.0.6 - 11/26/2019

- Fix `WORKSPACE_BUCKET` environment variable

Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.6`

## 0.0.5 - 11/16/2019

- Remove apt-get upgrade for security purposes

Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.5`

## 0.0.4 - 10/18/2019

- Fix a bug in google_sign_in.js
- Fix WORKSPACE_NAME environment variable
  
Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.4`

## 0.0.3 - 10/09/2019

Check Metadata and lock interval on extension are now staggered

## 0.0.2 - 10/01/2019

Lint the .js extension files

## 0.0.1 - 08/21/2019

- Extends Ubuntu base image
- Add google-cloud-sdk
- Add Python 3.7
- Add pip
- Add conda
- Add Jupyter & JupyterLab
- Add Leonardo customizations/extensions

Image URL: `us.gcr.io/broad-dsp-gcr-public/terra-jupyter-base:0.0.1`
