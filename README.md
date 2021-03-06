# Supplementary code

## How to reproduce:

1. Place a sample MRI data from Alzheimer Disease Big Data DREAM Challenge to contrib/sample_mri_data

2. Place ADNI_Training_Q3_new.csv to contrib/sample_basic_data/

3. Place unzipped Synapse code at https://www.synapse.org/#!Synapse:syn8077016 to contrib/original_code

The contrib folder should look like:

contrib
contrib/sample_basic_data
contrib/sample_basic_data/ADNI_Training_Q3_new.csv
contrib/sample_mri_data
contrib/sample_mri_data/training_baseline_data.csv
contrib/sample_mri_data/training_image_tables
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504/tables
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504/tables/right_surface
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504/tables/right_surface/sulcus_shapes.csv
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504/tables/right_surface/label_shapes.csv
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504/tables/volumes_FreeSurfer_labels.csv
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504/tables/left_surface
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504/tables/left_surface/sulcus_shapes.csv
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504/tables/left_surface/label_shapes.csv
contrib/sample_mri_data/training_image_tables/9bd97e848f4090d03b4e2975eed4a504/tables/thickinthehead_FreeSurfer_labels.csv
contrib/processed_data
contrib/processed_data/ADNI_Final_Q3_new.csv_matlab.csv
contrib/processed_data/ADNI_Training_Q3_new.csv_matlab.csv
contrib/processed_data/ADNI_Leaderboard_Q3_new.csv_matlab.csv
contrib/original_code
contrib/original_code/covar_add_variance.m
contrib/original_code/prepareMatlabInput.pl
contrib/original_code/ADNI_Final_Q3_new.csv_matlab.csv
contrib/original_code/ADNI_Training_Q3_new.csv
contrib/original_code/AD3_final.m
contrib/original_code/prepareMatlabLeaderboard.pl
contrib/original_code/ADNI_Training_Q3_new.csv_matlab.csv
contrib/original_code/ADNI_Leaderboard_Q3_new.csv_matlab.csv
contrib/original_code/prepareMatlabFinal.pl
contrib/original_code/gpr_prediction.m

Consider the size of these data, we cannot provide them through GitHub. Please download from Synpase website and put them here.

4. Run the IPython notebook.

## How to perform network analysis

Unfortunately, Cytoscape does not have an intuitive way to perform network analysis. We used the cytoscape.script in the root folder to analyze our network decomposition. Use cytoscape -S cytoscape.script will generate one round of decomposition. Use bash or other tools to repeat the process.

The network file can be import from network/complete/original.csv

The analysis requires Cytoscape and clusterMaker2.
