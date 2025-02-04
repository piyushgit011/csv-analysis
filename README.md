# Ayar Labs Unified Search Platform

## Architecture Overview

### 1. System Components

#### Core Components:
- **SmartDataLoader**: Handles data ingestion and preprocessing
- **SchemaAnalyzer**: Analyzes and maintains data schema information
- **SemanticQueryAnalyzer**: Processes natural language queries using LLM
- **SmartDataProcessor**: Processes and filters data based on query analysis
- **EnhancedVisualizer**: Creates dynamic visualizations

#### Technology Stack:
- Frontend: Streamlit
- Backend Processing: Python, Pandas
- Query Understanding: LangChain 
- Visualization: Plotly
- Data Storage: CSV Files

### 2. Data Flow

1. **Data Ingestion**
   - CSV files are loaded from the 'data' directory
   - Automatic preprocessing and cleaning
   - Schema generation and analysis

2. **Query Processing**
   - Natural language query input
   - Multi-step semantic analysis using GPT-4
   - Query intent extraction
   - Filter generation

3. **Data Processing**
   - Semantic filtering
   - Column selection and highlighting
   - Data transformation for visualization

4. **Visualization**
   - Dynamic chart generation
   - Interactive data exploration
   - Export capabilities

## Adding New Data

### Process for Adding New Data:
1. Place new CSV files in the 'data' directory
2. System automatically:
   - Detects new files
   - Preprocesses data
   - Generates schema
   - Makes data available for querying

### Data Requirements:
- File Format: CSV
- Location: 'data' directory
- Column Names: Should be clear and descriptive
- Date Formats: Supported formats include:
  - YYYY-MM-DD
  - DD/MM/YYYY
  - MM/DD/YYYY
  - YYYY-MM-DD HH:MM:SS

### Automatic Data Processing:
- Column name standardization
- Date format standardization
- Numeric data type conversion
- String cleaning and standardization

## System Features

### 1. Natural Language Query Support
- Free-form text queries
- Context-aware query understanding
- Multi-dataset query capability

### 2. Intelligent Data Processing
- Automatic schema detection
- Smart filtering and aggregation
- Column type inference
- Missing data handling

### 3. Visualization Capabilities
- Dynamic chart generation
- Multiple visualization types:
  - Line charts
  - Bar charts
  - Scatter plots
  - Box plots
  - Heatmaps

### 4. Data Export
- CSV export functionality
- Filtered data download
- Complete dataset access

## Maintenance and Updates

### Adding New Data Sources:
1. Add new CSV files to 'data' directory
2. Restart application (if running)
3. System automatically incorporates new data

### Updating Existing Data:
1. Replace existing CSV files
2. System automatically reloads on next startup

### Schema Updates:
- Automatic schema regeneration
- No manual schema updates required
- Dynamic column type detection

## Technical Details

### Key Classes:

1. **SmartDataLoader**
   - CSV file loading
   - Data preprocessing
   - Type inference

2. **SchemaAnalyzer**
   - Schema generation
   - Column analysis
   - Statistics calculation

3. **SemanticQueryAnalyzer**
   - Query understanding
   - Filter generation
   - Visualization recommendations

4. **SmartDataProcessor**
   - Data filtering
   - Column selection
   - Data transformation

5. **EnhancedVisualizer**
   - Chart generation
   - Interactive visualization
   - Multiple chart types

### Error Handling:
- Robust error catching
- Informative error messages
- Graceful failure handling

### Performance Considerations:
- Efficient data loading
- Smart caching using session state
- Optimized data processing

## Future Enhancements

1. Potential Additions:
   - Support for more file formats
   - Advanced visualization options
   - Real-time data updates
   - Custom query templates

2. Scalability Improvements:
   - Database integration
   - Parallel processing
   - Advanced caching

## Support and Maintenance

### Common Tasks:
1. Adding new data: Place CSV in 'data' directory
2. Updating data: Replace existing CSV files
3. Modifying visualizations: Update EnhancedVisualizer class
4. Customizing queries: Modify SemanticQueryAnalyzer prompts

### Troubleshooting:
- Check logs for detailed error messages
- Verify CSV file format
- Ensure proper column naming
- Validate date formats
