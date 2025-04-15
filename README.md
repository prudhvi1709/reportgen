# ReportGen

ReportGen is an automated letter generation tool designed for compliance and regulatory environments. It streamlines the creation of compliance-related documents while ensuring accuracy and adherence to regulations.

## For Users

### Overview

ReportGen is hosted at [reportgen.straive.app](https://reportgen.straive.app). It offers:

1. **VAPT Test Report Generation**: Generate a Vulnerability Assessment and Penetration Testing (VAPT) report from pre-loaded data.
2. **Custom Report Generation**: Upload your own VAPT Excel report for analysis.

### How to Use

1. Visit [reportgen.straive.app](https://reportgen.straive.app)
2. Log in to LLM Foundry if prompted
3. Choose one of the following options:
   - Click "Generate" under "VAPT test" to use pre-loaded data
   - Click "Upload your Excel file here" under "Custom Report" to use your own data
4. View the generated report, including:
   - Executive Summary
   - Security and Threat Prevention analysis
   - Network Utilization charts
   - AI-generated recommendations

### Features

- Interactive charts for bandwidth and session usage
- AI-powered recommendations based on report data
- Responsive design for various screen sizes
- Dark mode toggle

## For Developers

### Project Structure

- `index.html`: Main HTML file
- `script.js`: Core JavaScript functionality
- `img/`: Directory for images used in the report

### Adding New Demos

To add a new demo:

1. Update the `#demos` section in `index.html`
2. Create a new Excel file (e.g., `new-demo.xlsx`) with the required data structure:
   - Include a "Summary" sheet with key-value pairs
   - Add additional sheets for specific data sections
3. Update the `vaptReport` function in `script.js` to handle the new data structure if needed
4. Modify the chart generation code if the new demo requires different visualizations

### Technologies Used

- HTML5, CSS3 (Bootstrap 5.3.3)
- JavaScript (ES6+)
- lit-html for templating
- Chart.js for data visualization
- XLSX library for Excel file parsing
- Marked for Markdown parsing
- LLM Foundry API for AI-generated recommendations

### Development Setup

1. Clone the repository
2. Serve the project using a local web server (e.g., `python -m http.server`)
3. Open `http://localhost:8000` in your browser

### API Integration

The project uses the LLM Foundry API for generating recommendations. Ensure you have the necessary credentials and update the token retrieval logic in `script.js` if needed.

### Customization

- Modify the `vaptReport` function in `script.js` to change the report structure
- Update styles in `index.html` to customize the appearance
- Adjust chart configurations in `script.js` for different visualizations
