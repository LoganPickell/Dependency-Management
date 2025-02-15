# <p align="center">Dependency Management</p>

---

## <p align="center">Purpose of the script</p>

##### The script visualizes population density on an interactive 3D globe. The purpose is to provide an insightful, interactive way to explore global population distribution 🌍

---

## <p align="center"> Steps followed</p>

##### 1. Created globe.py (copied from assignment)
##### 2. Create virtual environment to control dependencies
    python -m venv venv
##### 3. Manually install each dependency missing from globe.py
    pip install ...
##### 4. Generated all_requirements.txt
    pip freeze > all_requirements.txt
##### 5. Created and checked dependency_tree.txt
    pipdeptree > dependency_tree.txt
##### 6. Removed all installed packages
    pip uninstill -y -r all_requirements.txt
##### 7. Created a minimal requirements txt file
    pipreqs . --force
##### 8. Reinstalled from requirements.txt
    pip install -r requirements.txt

---

# <p align="center">Output of pipdeptree</p>

geopandas==1.0.1
  - numpy [required: >=1.22, installed: 2.2.3]
  - packaging [required: Any, installed: 24.2]
  - pandas [required: >=1.4.0, installed: 2.2.3]
    - numpy [required: >=1.26.0, installed: 2.2.3]
    - python-dateutil [required: >=2.8.2, installed: 2.9.0.post0]
      - six [required: >=1.5, installed: 1.17.0]
    - pytz [required: >=2020.1, installed: 2025.1]
    - tzdata [required: >=2022.7, installed: 2025.1]
  - pyogrio [required: >=0.7.2, installed: 0.10.0]
    - certifi [required: Any, installed: 2025.1.31]
    - numpy [required: Any, installed: 2.2.3]
    - packaging [required: Any, installed: 24.2]
  - pyproj [required: >=3.3.0, installed: 3.7.0]
    - certifi [required: Any, installed: 2025.1.31]
  - shapely [required: >=2.0.0, installed: 2.0.7]
    - numpy [required: >=1.14,<3, installed: 2.2.3]
pipdeptree==2.25.0
  - packaging [required: >=24.1, installed: 24.2]
  - pip [required: >=24.2, installed: 25.0.1]
pipreqs==0.5.0
  - docopt [required: ==0.6.2, installed: 0.6.2]
  - ipython [required: ==8.12.3, installed: 8.12.3]
    - backcall [required: Any, installed: 0.2.0]
    - colorama [required: Any, installed: 0.4.6]
    - decorator [required: Any, installed: 5.1.1]
    - jedi [required: >=0.16, installed: 0.19.2]
      - parso [required: >=0.8.4,<0.9.0, installed: 0.8.4]
    - matplotlib-inline [required: Any, installed: 0.1.7]
      - traitlets [required: Any, installed: 5.14.3]
    - pickleshare [required: Any, installed: 0.7.5]
    - prompt_toolkit [required: >=3.0.30,<3.1.0,!=3.0.37, installed: 3.0.50]
      - wcwidth [required: Any, installed: 0.2.13]
    - Pygments [required: >=2.4.0, installed: 2.19.1]
    - stack-data [required: Any, installed: 0.6.3]
      - asttokens [required: >=2.1.0, installed: 3.0.0]
      - executing [required: >=1.2.0, installed: 2.2.0]
      - pure_eval [required: Any, installed: 0.2.3]
    - traitlets [required: >=5, installed: 5.14.3]
  - nbconvert [required: >=7.11.0,<8.0.0, installed: 7.16.6]
    - beautifulsoup4 [required: Any, installed: 4.13.3]
      - soupsieve [required: >1.2, installed: 2.6]
      - typing_extensions [required: >=4.0.0, installed: 4.12.2]
    - bleach [required: !=5.0.0, installed: 6.2.0]
      - webencodings [required: Any, installed: 0.5.1]
    - defusedxml [required: Any, installed: 0.7.1]
    - Jinja2 [required: >=3.0, installed: 3.1.5]
      - MarkupSafe [required: >=2.0, installed: 3.0.2]
    - jupyter_core [required: >=4.7, installed: 5.7.2]
      - platformdirs [required: >=2.5, installed: 4.3.6]
      - pywin32 [required: >=300, installed: 308]
      - traitlets [required: >=5.3, installed: 5.14.3]
    - jupyterlab_pygments [required: Any, installed: 0.3.0]
    - MarkupSafe [required: >=2.0, installed: 3.0.2]
    - mistune [required: >=2.0.3,<4, installed: 3.1.1]
    - nbclient [required: >=0.5.0, installed: 0.10.2]
      - jupyter_client [required: >=6.1.12, installed: 8.6.3]
        - jupyter_core [required: >=4.12,!=5.0.*, installed: 5.7.2]
          - platformdirs [required: >=2.5, installed: 4.3.6]
          - pywin32 [required: >=300, installed: 308]
          - traitlets [required: >=5.3, installed: 5.14.3]
        - python-dateutil [required: >=2.8.2, installed: 2.9.0.post0]
          - six [required: >=1.5, installed: 1.17.0]
        - pyzmq [required: >=23.0, installed: 26.2.1]
        - tornado [required: >=6.2, installed: 6.4.2]
        - traitlets [required: >=5.3, installed: 5.14.3]
      - jupyter_core [required: >=4.12,!=5.0.*, installed: 5.7.2]
        - platformdirs [required: >=2.5, installed: 4.3.6]
        - pywin32 [required: >=300, installed: 308]
        - traitlets [required: >=5.3, installed: 5.14.3]
      - nbformat [required: >=5.1, installed: 5.10.4]
        - fastjsonschema [required: >=2.15, installed: 2.21.1]
        - jsonschema [required: >=2.6, installed: 4.23.0]
          - attrs [required: >=22.2.0, installed: 25.1.0]
          - jsonschema-specifications [required: >=2023.03.6, installed: 2024.10.1]
            - referencing [required: >=0.31.0, installed: 0.36.2]
              - attrs [required: >=22.2.0, installed: 25.1.0]
              - rpds-py [required: >=0.7.0, installed: 0.22.3]
              - typing_extensions [required: >=4.4.0, installed: 4.12.2]
          - referencing [required: >=0.28.4, installed: 0.36.2]
            - attrs [required: >=22.2.0, installed: 25.1.0]
            - rpds-py [required: >=0.7.0, installed: 0.22.3]
            - typing_extensions [required: >=4.4.0, installed: 4.12.2]
          - rpds-py [required: >=0.7.1, installed: 0.22.3]
        - jupyter_core [required: >=4.12,!=5.0.*, installed: 5.7.2]
          - platformdirs [required: >=2.5, installed: 4.3.6]
          - pywin32 [required: >=300, installed: 308]
          - traitlets [required: >=5.3, installed: 5.14.3]
        - traitlets [required: >=5.1, installed: 5.14.3]
      - traitlets [required: >=5.4, installed: 5.14.3]
    - nbformat [required: >=5.7, installed: 5.10.4]
      - fastjsonschema [required: >=2.15, installed: 2.21.1]
      - jsonschema [required: >=2.6, installed: 4.23.0]
        - attrs [required: >=22.2.0, installed: 25.1.0]
        - jsonschema-specifications [required: >=2023.03.6, installed: 2024.10.1]
          - referencing [required: >=0.31.0, installed: 0.36.2]
            - attrs [required: >=22.2.0, installed: 25.1.0]
            - rpds-py [required: >=0.7.0, installed: 0.22.3]
            - typing_extensions [required: >=4.4.0, installed: 4.12.2]
        - referencing [required: >=0.28.4, installed: 0.36.2]
          - attrs [required: >=22.2.0, installed: 25.1.0]
          - rpds-py [required: >=0.7.0, installed: 0.22.3]
          - typing_extensions [required: >=4.4.0, installed: 4.12.2]
        - rpds-py [required: >=0.7.1, installed: 0.22.3]
      - jupyter_core [required: >=4.12,!=5.0.*, installed: 5.7.2]
        - platformdirs [required: >=2.5, installed: 4.3.6]
        - pywin32 [required: >=300, installed: 308]
        - traitlets [required: >=5.3, installed: 5.14.3]
      - traitlets [required: >=5.1, installed: 5.14.3]
    - packaging [required: Any, installed: 24.2]
    - pandocfilters [required: >=1.4.1, installed: 1.5.1]
    - Pygments [required: >=2.4.1, installed: 2.19.1]
    - traitlets [required: >=5.1, installed: 5.14.3]
  - yarg [required: ==0.1.9, installed: 0.1.9]
    - requests [required: Any, installed: 2.32.3]
      - certifi [required: >=2017.4.17, installed: 2025.1.31]
      - charset-normalizer [required: >=2,<4, installed: 3.4.1]
      - idna [required: >=2.5,<4, installed: 3.10]
      - urllib3 [required: >=1.21.1,<3, installed: 2.3.0]
plotly==6.0.0
  - narwhals [required: >=1.15.1, installed: 1.26.0]
  - packaging [required: Any, installed: 24.2]
tinycss2==1.4.0
  - webencodings [required: >=0.4, installed: 0.5.1]

---
# <p align="center">Observations or Issues</p>

No issues, I enjoyed the pipreqs . --force option to create a minimal requirements.txt. I plan to start using this, I think it's much cleaner than having 500 dependencies. 