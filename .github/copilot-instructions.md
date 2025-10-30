# Copilot Instructions for Bakery Project

## Project Overview
This is a German-language data science project focused on weather data analysis using Jupyter notebooks. The project demonstrates statistical analysis techniques including descriptive statistics, hypothesis testing, and data visualization.

## Key Architecture & Patterns

### Data Analysis Workflow
- **Primary notebook**: `List.ipynb` contains comprehensive weather data analysis
- **Data source**: External CSV from opencampus-sh GitHub repository (weather data)
- **Analysis pipeline**: Load → Clean → Analyze → Visualize → Test statistical significance
- **Output**: Generated PNG visualizations saved to project root

### Code Structure Patterns
- German comments and variable names throughout (e.g., "Wetterdaten Analyse", "durchschnittliche Gesamttemperatur")
- Comprehensive statistical analysis with both descriptive and inferential statistics
- Multi-panel matplotlib visualizations with customized styling
- Structured analysis sections marked with ASCII art separators (`"=" * 70`)

### Dependencies & Environment
- **Core libraries**: pandas, numpy, matplotlib, scipy.stats, requests
- **Notebook environment**: Python 3.12.1 with Jupyter
- **No requirements.txt**: Dependencies managed through notebook environment
- **Output files**: Generated visualizations (`.png`) are gitignored

## Development Conventions

### Language & Localization
- **Primary language**: German for comments, variables, and output text
- **Variable naming**: German descriptive names (e.g., `df_july`, `overall_avg`, `may_avg`)
- **Output formatting**: German month names and statistical terminology

### Statistical Analysis Patterns
- Standard workflow: descriptive stats → visualization → hypothesis testing
- Use of scipy.stats for t-tests with Cohen's d effect size calculations
- Comprehensive result reporting with significance levels and effect size interpretation
- Multi-plot visualizations combining boxplots, histograms, and bar charts

### File Organization
- Single notebook approach for complete analysis
- Generated outputs saved to project root (not in subdirectories)
- Standard Python .gitignore for compiled files and cache

## Working with this Project

### Running Analysis
- Execute `List.ipynb` cells sequentially - the notebook is self-contained
- External data is fetched automatically via requests/pandas
- Visualizations are both displayed and saved as PNG files

### Adding New Analysis
- Follow the existing section structure with ASCII separators
- Maintain German language conventions for consistency
- Include both descriptive and inferential statistics where appropriate
- Generate accompanying visualizations for key findings

### Data Sources
- Weather data: External CSV from opencampus-sh repository
- Data loading pattern: `requests.get()` + `pd.read_csv()` with StringIO buffer
- Automatic date parsing and month extraction for temporal analysis