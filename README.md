# MakeYourData

## Overview

"MakeYourData" is a simple Python app built using **Streamlit** that allows you to create synthetic datasets by interactively drawing points on a canvas. With this tool, you can visually generate data by clicking on the canvas and choosing different colors for the points. It's ideal for testing data analysis, machine learning models, or creating small toy datasets for various applications.

### Key Features
- **Interactive Drawing**: Draw points on a canvas by clicking, and they will automatically be added to the dataset.
- **Color Selection**: Choose between two colors (red or blue) for the points you draw.
- **Data Export**: The app generates a synthetic dataset of points (X, Y coordinates and color) that you can view and export.
- **Canvas Reset**: A button to clear the canvas and reset the dataset.

## How It Works

1. **Select the Color**: You can choose between **red** or **blue** as the color of the points you draw.
2. **Draw on the Canvas**: Use the canvas to click and generate points. Each click will create a point at the location you clicked, and its coordinates will be recorded in the dataset.
3. **Dataset**: The app will track the generated points (X, Y coordinates) and the selected color for each point.
4. **Clear Data**: You can clear the canvas and start over by clicking the "Clean Data" button.
5. **View and Export the Dataset**: The generated points are displayed in a table, which you can review and export for further analysis or use.

## Installation

To run this app locally, you'll need to have Python installed along with the following libraries:

- **Streamlit**: For building the web app.
- **Pandas**: For handling and displaying the generated dataset.
- **Streamlit Drawable Canvas**: For the interactive drawing functionality.
- **Matplotlib**: For displaying any additional charts or plots.

To install the required dependencies, run the following commands:

```bash
pip install streamlit pandas streamlit-drawable-canvas matplotlib
```

## How to Run

1. Clone or download this repository to your local machine.
2. Save the code in a Python file, for example `toy_data_generator.py`.
3. In your terminal, navigate to the directory where the file is saved.
4. Run the Streamlit app with the following command:

```bash
streamlit run toy_data_generator.py
```

The app will open in your browser where you can start generating your toy dataset.

## Usage

1. **Choose a color**: Select between **red** or **blue** using the radio button in the sidebar.
2. **Draw points**: Click on the canvas to create points. Each point will have its X, Y coordinates stored along with its selected color.
3. **View dataset**: The table below the canvas will show your generated dataset with columns `X`, `Y`, and `Color`.
4. **Clean data**: Click the "Clean Data" button to clear the canvas and reset the dataset.

## Example Output

Once you draw some points, the dataset will appear below the canvas:

| X    | Y    | Color |
|------|------|-------|
| 120  | 150  | blue  |
| 200  | 250  | red   |
| 300  | 350  | blue  |

## Notes

- This app is designed for quick data generation and exploration, making it useful for testing algorithms, visualization, or other lightweight data-related tasks.
- If you need to save the dataset, you can manually export the DataFrame from Streamlit or add functionality for downloading the data.

## License

This app is open-source and available for modification under the [MIT License](LICENSE).

---

Created by [CLL](https://github.com/CllsPy)
