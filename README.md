# AFIDs-Data

This dataset contains sets of images and ground truth AFID (anatomical fiducial) placements for those images.

For the purposes of evaluating two proposed dataset structures, the datasets are structured either:

- As single BIDS datasets (`afids-{dataset}`) with placements included under `derivatives/afids_groundtruth`
- As matched pairs of BIDS datasets (`afids-{dataset}-separate`): one with the images (`bids-{dataset}` and one with the AFID placements `afids-groundtruth-{dataset}`

In either case, the datasets are distributed using DataLad. You can install all datasets using `datalad install -r git@github.com:tkkuehn/afids-data-datalad.git`, and get individual images using `datalad get {image_path}`. Some images may require authentication or other steps; such cases are documented in the dataset READMEs.
