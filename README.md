# nerfstudio-template
Template repository for creating and registering methods in Nerfstudio.

## File Structure

We recommend the following file structure:

```
├── my_method
│   ├── __init__.py
│   ├── my_config.py
│   ├── custom_pipeline.py [optional]
│   ├── custom_model.py [optional]
│   ├── custom_field.py [optional]
│   ├── custom_datamanger.py [optional]
│   ├── custom_dataparser.py [optional]
│   ├── ...
├── pyproject.toml
```

## Registering with NerfStudio

```
conda activate nerfstudio
cd nerfstudio-template
pip install -e .
ns-install-cli
```

## Running the new method
```
ns-train nerfstudio-template --data [PATH]
```