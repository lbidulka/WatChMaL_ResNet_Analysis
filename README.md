# WatChMaL_ResNet_Analysis
Results and data plotting for the forthcoming WatChMaL ResNet particle identification paper.

## Requirements & Setup:
In its current form, this repo is intended to be run on the TRIUMF ML1 machine in the same recommended singularity image as the [main WatChMaL code](https://github.com/WatChMaL/WatChMaL)  (/fast_scratch/triumfmlutils/containers/base_ml_recommended.simg) but it should be easily transferable to another environment if needed. 

If you will be running this on ML1 in the recommended base image, all you need to do is clone this repo and run its notebooks without any changes. 

If my own `/home/lbidulka` directory has been removed or changed at the time you read this, you will likely just need to modify the sys paths in this repos notebooks to refer to an up-to-date main WatChMaL repo location. On ML1, you could likely use `/home/nprouse`, or use your own main repo download location if you want.

## Notebooks:
### watchmal_paper_4class_plotting.ipynb
- Contains plots for all 3 tasks of the 4-class model: e vs gamma, e vs muon, and e vs pi0. For each task there are ROC curves as well as binned true_momentum, dwall, towall, zenith and azimuth plots.
### watchmal_paper_e_gamma_plotting.ipynb
- Contains plots for the 1 task of the 2-class model: e vs gamma. For this task, the 2-class and 4-class results are plotted together on ROC curves as well as binned true_momentum, dwall, towall, zenith and azimuth plots.
### watchmal_paper_event_plotting.ipynb
- Contains loading and plotting of the short IWCD tank geometry both in a 3D and unrolled manner. Also plots an example unrolled test event sample. 

## Results Folders:
### 4_class_results
- Contains 3 sub-folders, one for each task e vs gamma, e vs muon, and e vs pi0. Within each task sub-folder, there are jpgs for each plot produced by watchmal_paper_4class_plotting.ipynb.
### e_gamma_combined_results
- Contains jpgs for each plot produced by watchmal_paper_e_gamma_plotting.ipynb for the e vs gamma task.
