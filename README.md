# 🎓 Student Placement Analytics Dashboard

A beautiful, interactive dashboard built with Streamlit and Plotly to visualize student placement data. Features a modern dark theme inspired by Power BI with rich, interactive visualizations.

![Dashboard Preview](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=Streamlit&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)

## ✨ Features

- 📊 **Interactive Visualizations**: Multiple chart types including bar charts, donut charts, area charts, and treemaps
- 🎨 **Modern Dark Theme**: Professional Power BI-inspired dark mode design with gradient accents
- 🔍 **Advanced Filtering**: Filter data by Year, Branch, and Company with real-time updates
- 📈 **Comprehensive Analytics**:
  - Branch-wise placement distribution
  - Top recruiting companies analysis
  - Year-over-year placement trends
  - Top performers and key metrics
- 🔎 **Smart Search**: Search functionality across student names, roll numbers, and companies
- 💾 **Data Export**: Download filtered data as CSV
- 📱 **Responsive Design**: Works seamlessly on different screen sizes

## 🚀 Demo

The dashboard provides insights into:
- Total students placed across all years
- Number of recruiting companies
- Branch-wise placement statistics
- Top recruiting companies
- Yearly placement trends
- Interactive data exploration

## 📋 Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/placement-dashboard.git
   cd placement-dashboard
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv streamlit_env
   ```

3. **Activate the virtual environment**
   - Windows:
     ```bash
     streamlit_env\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source streamlit_env/bin/activate
     ```

4. **Install required packages**
   ```bash
   pip install -r requirements.txt
   ```

## 📦 Required Packages

```txt
streamlit
pandas
plotly
```

Create a `requirements.txt` file with the above packages or install them individually:
```bash
pip install streamlit pandas plotly
```

## 🎯 Usage

1. **Prepare your data**
   - Ensure your `data.csv` file is in the same directory as `app.py`
   - The CSV should have columns: `Year`, `S.No`, `Roll No`, `Name of the Student`, `Branch`, `Name of the Employer`

2. **Run the dashboard**
   ```bash
   streamlit run app.py
   ```

3. **Access the dashboard**
   - The application will automatically open in your default web browser
   - Default URL: `http://localhost:8501`

## 📊 Data Format

Your `data.csv` should follow this structure:

```csv
Year,S.No,Roll No,Name of the Student,Branch,Name of the Employer
2024-25,1,217Z1R0008,John Doe,CSE,ABC Company
2024-25,2,217Z1R0009,Jane Smith,ECE,XYZ Corp
...
```

## 🎨 Dashboard Sections

### 1. **Key Metrics Cards**
- Total Students Placed
- Number of Companies
- Total Branches
- Academic Years Covered

### 2. **Branch Analysis**
- Interactive bar chart showing placements by branch
- Donut chart for branch distribution percentage

### 3. **Company Insights**
- Top 15 recruiting companies horizontal bar chart
- Treemap visualization of top 10 companies

### 4. **Yearly Trends**
- Area chart showing placement trends over years
- Top performers summary cards
- Average placements per year

### 5. **Year-wise Comparison**
- Bar chart for each year's placements
- Pie chart comparing top 5 companies vs others

### 6. **Data Table**
- Searchable, filterable data table
- Download option for filtered data

## 🎛️ Customization

### Changing Colors
Edit the CSS in `app.py` to customize the color scheme:
```python
st.markdown("""
    <style>
    .main {
        background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
    }
    </style>
""", unsafe_allow_html=True)
```

### Adding New Visualizations
Add new charts by following the Plotly Express pattern:
```python
fig = px.bar(data, x="column1", y="column2", title="Your Title")
st.plotly_chart(fig, use_container_width=True)
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

Your Name
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)

## 🙏 Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Visualizations powered by [Plotly](https://plotly.com/)
- Data analysis with [Pandas](https://pandas.pydata.org/)
- Inspired by Power BI's modern dashboard design

## 📸 Screenshots

### Dashboard Overview
![Dashboard Overview](screenshots/dashboard.png)

### Branch Analysis
![Branch Analysis](screenshots/branch-analysis.png)

### Company Insights
![Company Insights](screenshots/company-insights.png)

## 🐛 Known Issues

- None at the moment. Please report any issues you find!

## 🔮 Future Enhancements

- [ ] Add more chart types (scatter plots, box plots)
- [ ] Implement user authentication
- [ ] Add data export in multiple formats (Excel, PDF)
- [ ] Include salary statistics
- [ ] Add department-wise comparison
- [ ] Implement dark/light theme toggle

## 📞 Support

For support, email your-email@example.com or open an issue in the repository.

---

Made with ❤️ using Streamlit and Plotly
