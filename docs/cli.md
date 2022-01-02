# Command-line Interface

The system supports command line mode (without triggering the GUI) for batch processing. But this should only be used for a batch of images of similar qualities. In general, there is no guarantee of the correctness of the final output without human intervention.

```
./Cellogram -i {PATH_TO_IMAGE} -c -s {PATH_TO_JSON_SETTINGS}
```

We also prepared a MATLAB script to invoke this batch mode at `script/batch_cellgram.m`.

Especially, the JSON file can override all the settings used in the GUI analysis. Here are the default values for some of the settings:
```
json default_analysis_settings = R”({
    “scaling”: 0.098,
    “zscaling”: 0.5,
    “E”: 13.578,
    “I”: 0.5,
    “L”: 3.0,
    “eps”: 0.32967033982276917,
    “formulation”: “LinearElasticity”,
    “image_from_pillars”: false,
    “nu”: 0.49,
    “padding_size”: 25.0,
    “displacement_threshold”: 0.18,
    “relative_threshold”: true,
    “mesh_size”: 0.15,
    “thickness”: 30.0,
    “mesh_gradation”: 1.2
    })“_json;
```
