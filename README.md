# fmp_data_munge

## Description
This script takes a spreadsheet of FileMaker Pro data and adds new columns to the spreadsheet based on the data in the existing columns and API calls to LCNAF and VIAF.

## Installation
1. Create a directory to hold the project and navigate to it (you can name it what you like):
    ```shell
    mkdir fmp_data_munge_outer
    cd fmp_data_munge_outer
    ```
2. Copy the repository url and clone the repository:
    ```shell
    git clone [repository url]
    ```
3. Create a virtual environment in the root directory of the project (recommended):
    ```shell
    python -m venv [virtual environment name]
    ```
4. If you created a virtual environment, activate it using the following command:
    ```shell
    source [virtual environment name]/bin/activate
    ```
5. Install the required packages using the following command:
    ```shell
    pip install -r requirements.txt
    ```

## Usage
1. If you have not already done so, activate the virtual environment (if you created one):
    ```shell
    source [virtual environment name]/bin/activate
    ```
2. Run the script using the following command:
    ```shell
    python fmp_data_munge.py [input file path] [output file path]
    ```
    The input and output files must be in csv format. If the output directory does not exist, the script will create it. If the output file already exists, the script will overwrite it. If no output file path is provided, the script will create a new file in ../output/ named "processed_data.csv". If there are spaces in the file path, enclose the path in quotes.

    example:
    ```shell
    python fmp_data_munge.py "My Files/input_data.csv" "My Files/output_data.csv"
    ```

## Contributing
If you would like to contribute to this project, please follow these steps:
1. Fork the repository.
2. Create a new branch.
3. Make your changes and commit them.
4. Push your changes to your forked repository.
5. Submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE).