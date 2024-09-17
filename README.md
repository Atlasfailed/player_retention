# Player Retention Analysis Project

This project analyzes player retention and engagement for a game using match data. It processes player statistics, categorizes players, and generates visualizations to provide insights into player behavior and game performance.

## Features

- Player categorization based on engagement levels
- Retention rate analysis across different player categories
- Matchmaking quality assessment
- Player engagement patterns analysis (hourly and daily)
- Automated HTML report generation with interactive charts

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/player-retention-analysis.git
   cd player-retention-analysis
   ```

2. Install the required dependencies:
   ```
   pip install pandas numpy plotly
   ```

## Usage

1. Ensure your data files (`matches.parquet` and `match_players.parquet`) are in the `data_source/prod/` directory.

2. Run the main script:
   ```
   python main.py
   ```

3. The script will generate an HTML report in the `player_retention/` directory named `player_analysis_report.html`.

## Project Structure

- `main.py`: The main script that orchestrates the analysis process.
- `data.py`: Contains functions for loading and processing data.
- `graphs.py`: Defines functions for creating visualizations.
- `report_generator.py`: Handles the generation of the HTML report.

## Generated Report

The generated HTML report includes the following visualizations:

1. Player Category Distribution
2. Average Total Matches by Player Category
3. Retention Rates by Player Category
4. Matchmaking Quality: Skill Gap Distribution
5. Player Engagement Patterns (Hourly and Daily)

Each chart is accompanied by an explanation of its significance and how to interpret the data.

## Customization

You can customize the analysis by modifying the following:

- Player categorization criteria in `categorize_players()` function
- Retention periods in `analyze_retention()` function
- Visualization styles in the `graphs.py` file

## Contributing

Contributions to improve the analysis or add new features are welcome. Please feel free to submit a pull request or open an issue to discuss potential changes.

## License

