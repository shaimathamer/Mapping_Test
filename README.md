# Mapping_Test
# Hospital Mapping Project

## Project Overview

This project aims to create a hospital mapping system for Uganda using satellite imagery and machine learning techniques. The project is divided into two parts:

1. **Part 1**: Dataset Creation - Collect and preprocess hospital and satellite imagery data.
2. **Part 2**: Model Training and Evaluation - Train a deep learning model to classify hospitals and non-hospitals based on satellite images.

### Final Deliverables:
- **Python Notebooks**:
  1. A self-contained and well-documented Python notebook implementing **Part 1** (Dataset Creation).
  2. A self-contained and well-documented Python notebook implementing **Part 2** (Model Training and Evaluation).
- **Presentation**: A presentation explaining the steps taken, decisions made, and showcasing the final results.
  ## Running the Code

### Google Colab
You can run this code in **Google Colab** without any special configuration.

#### Steps:
1. Download the **hospital location CSV file** (`hospitals.csv`) and place it in the `data/` folder.
2. The **satellite images** will be automatically saved to your **Google Drive**.
3. Other data will remain in memory and will be lost once the session ends.

### Google Earth Engine API
- If you want to **download satellite images** using the **Google Earth Engine API**, update the API configuration in the code.
- Ensure that you have the **necessary permissions** to use the **Google Earth Engine API**.

## Folder Setup
- Create a folder (e.g., `test_uncif`) to store your data.
- Download the **hospital location data** (in CSV format) and place it in the `data/` folder.
- **Satellite images** will be downloaded to your **Google Drive**.
- Other files and folders will remain in **memory** and be **lost** once the session is closed.

## Memory Considerations
- The project is optimized to run with **normal RAM** and does **not** require any special configuration or **payment** for cloud resources.
- Due to **memory constraints**, **only hospital data from Kampala (Uganda's capital)** is used for **map plotting**.
- **Non-hospital data from other regions of Uganda** may not fit into the available memory.

## Data Files
The required data files are located in the `data/` folder:

- **Hospital Location Data**:
- `hospitals.csv` (contains latitude and longitude of hospitals in Uganda).
- **Satellite Images**:
-  Downloaded using
-  **Google Earth Engine** and saved to
-  **Google Drive**.

## Final Notes
- After running the code, the **satellite images** will be **saved** to your **Google Drive**.
- Other files, such as **hospital data**, will remain in **memory** and will be **lost** after the session ends.
- If you encounter **memory limitations**, the project has been optimized to use only the **necessary resources**.

## Folder Structure

The project is organized into the following folder structure:

```plaintext
Hospital_Mapping_Project/
├── data/
│   ├── hospitals.csv              # Hospital location data in CSV format
│   └── satellite_images/          # Folder containing satellite images
├── notebooks/
│   ├── dataset_creation.py        # Code for creating the dataset
│   └── model_training.py          # Code for training the model
├── output/                        # Folder for storing output data (maps, images, etc.)
├── MAPPING_TEST/                  # Folder containing processed images for training/testing
│   ├── undersample_non_hospital/  # Undersampled non-hospital images
│   ├── hospital_augmented/        # Augmented hospital images
│   ├── non_hospital/              # Non-hospital images
│   ├── hospital/                  # Hospital images
├── README.md                      # Project overview and instructions
