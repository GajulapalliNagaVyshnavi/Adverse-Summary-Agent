<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
</head>
<body>
    <h1> Adverse Event Summary Agent</h1>
    <p>This tool analyzes <strong>treatment-emergent adverse events (TEAEs)</strong> from a clinical trial comparing <strong>varenicline</strong> and <strong>placebo</strong>, and generates a comprehensive summary using <strong>OpenAI GPT models</strong>.</p>
    <div class="section">
        <h2>🔧 Setup Instructions</h2>
        <h3>1. Clone the Repository</h3>
        <pre><code>git clone https://github.com/your-username/ae-summary-agent.git
cd ae-summary-agent</code></pre> 
        <h3>2. Create Python Virtual Environment</h3>
        <pre><code>python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate</code></pre>        
        <h3>3. Install Dependencies</h3>
        <pre><code>pip install -r requirements.txt</code></pre>
        <p><strong>requirements.txt</strong> should include:</p>
        <pre><code>pandas
openai
python-dotenv
plotly
ipython</code></pre>        
        <h3>4. Add Your OpenAI API Key</h3>
        <p>Create a <code>.env</code> file and add the following line:</p>
        <pre><code>OPENAI_API_KEY=your-openai-api-key-here</code></pre>
        <p><strong>Important:</strong> Never expose your <code>.env</code> file publicly.</p>
    </div>
    <div class="section">
        <h2>🚀 How to Run</h2>
        <h3>1. Update Input File Path</h3>
        <p>Make sure your CSV file (e.g., <code>adverse data2.csv</code>) is in the correct location.</p>
        <pre><code>file_path = 'adverse data2.csv'</code></pre>
        <h3>2. Run the Script</h3>
        <pre><code>python .ipynb files</code></pre>
        <p>The script will preprocess your data, format it into a prompt, and use GPT to summarize the cardiovascular AEs.</p>
    </div>
    <div class="section">
        <h2>📌 Output</h2>
        <p>You will get a well-structured summary discussing trends, SAEs, frequency of events, and comparison between treatment groups.</p>
    </div>
    <div class="section">
        <h2>🧠 Agent Details</h2>
        <ul>
            <li><strong>Model:</strong> gpt-4o-mini</li>
            <li><strong>Temperature:</strong> 0.2</li>
            <li><strong>Domain:</strong> Clinical Trial AE Analysis</li>
            <li><strong>Framework:</strong> Python (with Pandas, OpenAI API)</li>
        </ul>
    </div>
    <div class="section">
        <h2>🛠️ Troubleshooting</h2>
        <ul>
            <li><strong>File Not Found?</strong> Ensure the path and filename are correct.</li>
            <li><strong>Environment Variables Not Working?</strong> Ensure <code>load_dotenv()</code> is called and <code>.env</code> file is in the working directory.</li>
            <li><strong>API Error?</strong> Check if your OpenAI key is valid and your usage quota isn't exceeded.</li>
        </ul>
    </div>
    <div class="section">
        <h2>✏️ Customize Prompts</h2>
        <p><strong>Note:</strong> You can modify the prompt inside the <code>generate_summary</code> function to fit your analysis goals. <em>Change the prompts according to your requirements.</em></p>
    </div>
    <div class="section">
        <h2>📬 Contact</h2>
        <p>Author: Gajulapalli Naga Vyshnavi<br>
        Contact: <a href="mailto:nvyshnavi36@gmail.com">nvyshnavi36@gmail.com</a><br>
        For any inquiries or issues, feel free to reach out.</p>
    </div>
</body>
</html>
