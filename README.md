# jsPsych Decision Making Experiment

(FOR ARCHIVAL PURPOSE)

Code for a behavioral experiment investigating decision-making under risk using jsPsych. Participants choose whether to accept or reject gambles involving potential monetary gains and losses.

## File Structure

-   `experiment*.html`: The main HTML files to run different versions/conditions of the experiment.
-   `jspsych/`: Contains the necessary jsPsych library files (plugins, core script, CSS).
-   `css/`: Contains custom CSS (`style.css`) for the experiment appearance.
-   `php/`: Contains PHP scripts (`write_data*.php`) for saving data when run on a server.

## Experiment Versions
Low and High payoff conditions 

## Running the Experiment
Two ways:
1.  Locally (Testing/Single Use):
    *   Download or clone this repository.
    *   Open one of the `experiment*.html` files directly in your web browser.
    *   Upon completion, the experiment data will be automatically downloaded as a `.csv` file.
    *   Pilot Mode: Append `?pilot` to the URL in your browser (e.g., `file:///path/to/experiment1.html?pilot`) to run with zero trial durations for quick testing.

2.  On a Server:
    *   Upload the entire project directory.
    *   Create a `data/` directory on the server at the same level as the `php/` directory.
    *   Ensure the web server has write permissions for the `php/write_data*.php` script to save files into that `data/` directory.
    *   Access the `experiment*.html` file via its web URL (e.g., `http://yourdomain.com/experiment_folder/experiment1.html`).
    *   Data will be sent to the corresponding PHP script and saved as a `.csv` file within the `data/` directory on the server.
    *   If the PHP saving fails, the script includes a fallback to download the data locally as a CSV.

Data is saved as a csv. This version requires the csv files to be cleaned before analysis.
