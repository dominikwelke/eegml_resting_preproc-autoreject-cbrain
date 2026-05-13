This repository contains the build and test information autoreject preprocessing pipeline in the EEGManyLabs RestingState spin-off project.
the container is meant to run on CBRAIN but can also be used locally.

## Container Building Instructions
```
git clone https://github.com/dominikwelke/eegml_resting_preproc-autoreject-cbrain.git
cd eegml_resting_preproc-autoreject-cbrain
docker build --no-cache -t eegml-autoreject .
```

## Container Testing/Running Instructions
```
subid=HajD0031  # or any other
docker run -v your/local/input/folder:/input -v your/local/output/folder:/output eegml-autoreject /input /output $subid
```
