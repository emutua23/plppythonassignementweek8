# plppythonassignementweek8
A  basic analysis of the CORD-19 research dataset and creating a simple Streamlit application to display your findings. 
# 🦠 CORD-19 Data Explorer

An interactive Streamlit web application for exploring COVID-19 research papers from the CORD-19 dataset.

## 🌟 Features

- **📊 Interactive Dashboard**: Real-time data filtering and visualization
- **📈 Dynamic Charts**: Publications timeline, journal analysis, and author distributions
- **🔤 Text Analysis**: Word frequency analysis from paper titles
- **📥 Data Export**: Download filtered datasets as CSV
- **🎯 Smart Filtering**: Filter by year, journal, source, and author count

## 🚀 Live Demo

[View the live application here](https://your-app-name.netlify.app)

## 📱 Screenshots

![Dashboard](https://via.placeholder.com/800x400?text=Dashboard+Screenshot)

## 🛠️ Technologies Used

- **Streamlit**: Interactive web framework
- **Plotly**: Interactive visualizations
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing

## 🏃‍♂️ Running Locally

### Prerequisites
- Python 3.8+
- pip package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/cord19-explorer.git
   cd cord19-explorer
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   streamlit run app.py
   ```

4. **Open your browser**
   Navigate to `http://localhost:8501`

## 🌐 Deployment

### Deploy to Netlify

1. **Fork this repository** to your GitHub account

2. **Connect to Netlify**:
   - Go to [Netlify](https://netlify.com)
   - Click "New site from Git"
   - Select your forked repository

3. **Configure build settings**:
   - Build command: `pip install -r requirements.txt && streamlit run app.py`
   - Publish directory: (leave empty)

4. **Deploy**: Netlify will automatically deploy your app

### Deploy to Heroku

1. **Create a Heroku app**:
   ```bash
   heroku create your-app-name
   ```

2. **Push to Heroku**:
   ```bash
   git push heroku main
   ```

3. **Open the app**:
   ```bash
   heroku open
   ```

### Deploy to Streamlit Cloud

1. **Push to GitHub**
2. **Go to [share.streamlit.io](https://share.streamlit.io)**
3. **Connect your repository**
4. **Deploy with one click**

## 📊 Dataset

This application uses sample data that mimics the structure of the CORD-19 dataset:

- **Papers**: ~5,000 sample COVID-19 research papers
- **Time Range**: 2019-2024
- **Sources**: PMC, WHO, arXiv, bioRxiv, medRxiv
- **Fields**: Titles, authors, journals, publication dates

For the actual CORD-19 dataset, visit: [CORD-19 Dataset](https://www.semanticscholar.org/cord19/download)

## 🎛️ Interactive Features

### Sidebar Controls
- **📅 Year Range Slider**: Filter papers by publication year
- **📚 Journal Selector**: Choose specific journals or view all
- **🗂️ Source Filter**: Filter by data source (PMC, WHO, etc.)
- **👥 Author Count Range**: Filter by collaboration size

### Visualizations
- **📈 Publication Timeline**: Interactive bar chart of papers over time
- **📊 Top Journals**: Horizontal bar chart of most productive journals
- **👥 Author Distribution**: Distribution of collaboration sizes
- **🗂️ Source Breakdown**: Pie chart of data sources
- **🔤 Word Frequency**: Most common words in paper titles

## 🔧 Configuration

### Environment Variables
Create a `.env` file for local development:
```env
STREAMLIT_SERVER_PORT=8501
STREAMLIT_SERVER_HEADLESS=true
```

### Customization
- Modify `app.py` to change the app structure
- Update `requirements.txt` for additional packages
- Edit styling in the CSS section of `app.py`

## 📈 Performance

The app is optimized for performance with:
- **@st.cache_data** decorators for data processing
- **Efficient filtering** with pandas operations
- **Interactive Plotly charts** with smooth animations
- **Responsive design** for mobile and desktop

## 🤝 Contributing

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature-name`
3. **Make your changes**
4. **Commit**: `git commit -m "Add feature"`
5. **Push**: `git push origin feature-name`
6. **Create a Pull Request**

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **CORD-19 Dataset**: Allen Institute for AI
- **Streamlit**: For the amazing web framework
- **Plotly**: For interactive visualizations
- **Open Source Community**: For the tools and libraries

## 📞 Contact

- **GitHub**: [yourusername](https://github.com/yourusername)
- **Email**: your-email@example.com
- **LinkedIn**: [Your Name](https://linkedin.com/in/yourprofile)

---

**⭐ If you found this project helpful, please star the repository!**

## 📚 Additional Resources

- [Streamlit Documentation](https://docs.streamlit.io/)
- [Plotly Documentation](https://plotly.com/python/)
- [CORD-19 Dataset Information](https://www.semanticscholar.org/cord19)
- [Pandas User Guide](https://pandas.pydata.org/docs/user_guide/index.html)

# CORD-19 Research Database Analysis

This project analyzes the **CORD-19 metadata dataset** (`metadata.csv`) to extract insights into publication trends, journal distributions, authorship, abstracts, and key terminology related to COVID-19 and associated research.

The workflow is implemented in a Jupyter notebook and Python scripts that load, clean, analyze, and visualize the dataset.

---

## 📊 Key Features
- **Robust Data Loading:** Multiple fallback strategies to handle CSV parsing errors and corrupted rows.
- **Data Quality Assessment:** Missing values analysis with visualizations.
- **Publication Timeline:** Trends from 1990–2024, with focus on 2010+.
- **Journal Analysis:** Top journals, diversity, and publication counts.
- **Title Analysis:** Distribution of title lengths, common words, and word clouds.
- **Abstract Analysis:** Length distributions and descriptive statistics.
- **Author Analysis:** Distribution of authors per paper, single vs. multi-author trends.
- **Source Analysis:** Breakdown of data sources (PMC, Medline, etc.).
- **File Availability:** Proportion of papers with PDF/PMC JSON files.

---

## 🛠️ Installation
Clone the repository and install dependencies:

```bash
git clone <repo-url>
cd cord19-analysis
pip install -r requirements.txt
