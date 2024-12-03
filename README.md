echo "# WhatsApp Chat Analyzer

This is a **Streamlit-based application** to analyze WhatsApp chat data. It helps users visualize key statistics and insights from their WhatsApp conversations, such as message counts, word frequency, emoji usage, most active users, and more.

## Features:
- **Overall Chat Stats**: Total messages, word count, media and links shared.
- **Monthly and Daily Timeline**: Visual representation of activity over time.
- **Most Active Users**: Find out who the most active participants are.
- **Word Cloud & Most Common Words**: See the most frequently used words and visualize them.
- **Emoji Analysis**: Analyzes the emoji usage in chats.
- **Activity Heatmap**: Visualize the chat activity based on days and time periods.

## Setup

### Prerequisites

Make sure you have Python 3.6+ installed and the following dependencies:

- Streamlit
- Pandas
- Matplotlib
- Seaborn
- WordCloud
- Emoji
- Urlextract
- Collections

You can install the required dependencies using \`pip\` by running:

\`\`\`bash
pip install -r requirements.txt
\`\`\`

Or, if you need to manually install dependencies, use:

\`\`\`bash
pip install streamlit pandas matplotlib seaborn wordcloud emoji urlextract
\`\`\`

You will also need to have a **WhatsApp chat export** in \`.txt\` format.

### File Structure

- \`app.py\`: Main file for the Streamlit app.
- \`helper.py\`: Contains helper functions for data analysis and visualizations.
- \`preprocessor.py\`: Preprocesses the chat data into a pandas DataFrame.
- \`stop_hinglish.txt\`: A text file containing stop words for cleaning the data (used during word cloud generation).

### Running the Application

To run the Streamlit app, execute the following command in your terminal:

\`\`\`bash
streamlit run app.py
\`\`\`

This will start the application on a local server (usually \`http://localhost:8501\`).

## How to Use

1. **Upload WhatsApp Chat File**: Use the sidebar to upload your WhatsApp \`.txt\` chat file.
2. **Select User**: Choose the user for analysis or select "Overall" to see group-wide statistics.
3. **View Analysis**: Click on "Show Analysis" to see the statistics, charts, and word cloud.

### Key Features in the App

- **Top Statistics**: View total messages, words, media shared, and links sent.
- **Monthly & Daily Timeline**: Interactive timeline to track the activity over time.
- **User Activity**: Visualize the most active users in the group and their communication patterns.
- **Word Cloud**: Generate a word cloud to see the most frequent words.
- **Emoji Analysis**: See which emojis are used the most by users.
- **Heatmap**: Activity heatmap to visualize the busiest times for chat activity.

### Sample Outputs:

1. **Top Statistics**:
   - Total messages, word count, media messages, and links shared by the selected user.
   
2. **Monthly Timeline**:
   - A line graph showing messages sent each month.

3. **Activity Map**:
   - A bar graph for the most active day and month.
   
4. **Word Cloud**:
   - A cloud representing the most common words used in the chat.

5. **Emoji Usage**:
   - A pie chart representing the most used emojis by a user/group.

## Files

### \`app.py\`

This file contains the core Streamlit application. It is responsible for uploading the chat data, processing it, and displaying various statistics and visualizations.

### \`helper.py\`

Contains the functions that process and analyze the WhatsApp data, such as:
- \`fetch_stats()\`: Fetches message stats like total messages, words, media, and links.
- \`most_busy_users()\`: Returns the most active users in the chat.
- \`create_wordcloud()\`: Generates a word cloud from chat messages.
- \`emoji_helper()\`: Analyzes and returns the usage of emojis.
- \`monthly_timeline()\`, \`daily_timeline()\`, \`activity_heatmap()\`, etc.: Various time-based visualizations.

### \`preprocessor.py\`

Contains the function \`preprocess()\`, which preprocesses the raw WhatsApp chat text file and extracts relevant information into a structured pandas DataFrame.

---

## Customizing the App

### Modify Stop Words

The word cloud functionality uses a custom stop words file (\`stop_hinglish.txt\`). You can edit this file to add or remove words as needed to refine the analysis.

### File Upload

You can modify the \`file_uploader\` section in \`app.py\` to support more file types or add additional file validation if needed.

---

## Troubleshooting

1. **App Not Loading**: Ensure all dependencies are correctly installed by running the \`pip install\` command.
2. **File Format Issues**: Ensure that the WhatsApp export file is in \`.txt\` format and follows the typical WhatsApp chat export structure.
3. **Missing \`stop_hinglish.txt\` File**: Make sure you have the \`stop_hinglish.txt\` file for word cloud generation.

## Contributing

Feel free to fork this project and submit issues or pull requests for bug fixes or feature enhancements.

## License

This project is open-source and available under the MIT License.
" > README.md

## Running Tests

To run tests, run the following command

```bash
  npm run test
```

