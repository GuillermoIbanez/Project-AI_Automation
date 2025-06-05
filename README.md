<div align="center">
  <h1>Guillermo Ibanez</h1>
  <p>
  </p>
  <h1>
    🚀 AI Automation | Customers Orders Extraction | Matching
</h1>
   <h1><img src="https://user-images.githubusercontent.com/74038190/221352987-68da234d-4d62-4e9d-9d7f-098dc657c2dc.gif" width="700" height="150"><h1>
</div>
 <div>
  <h3><a>Project for Arthur Weber as part of my Data Science & AI 4 months full time course</a></h3>

<h2>🎯 Objective</h2>
<p>We developed a proof-of-concept pipeline that applies modern natural language processing and semantic search techniques to streamline tender offers analysis. The core components include:</p>

<p><strong>Automated Text Extraction</strong><br>
Tender PDFs are parsed and cleaned to extract relevant product-related information.</p>

<p><strong>Item Structuring via GPT-4o-mini</strong><br>
A lightweight language model structures each item description, identifying the product, quantity, and unit, even when information is fragmented or embedded in a technical context.</p>

<p><strong>Semantic Product Matching</strong><br>
Using vector embeddings and cosine similarity, each tender item is compared to Arthur Weber's product database to retrieve top candidate matches.</p>

<p><strong>Final Validation with GPT</strong><br>
GPT is then used again to assess and validate the match, simulating the human verification process (see the picture below).</p>

<h2>⚡ Key Challenges</h2>
<p>The project was designed with real operational constraints in mind:</p>

<p><strong>Long, technical documents with inconsistent formatting</strong><br>
Documents often vary significantly in structure and presentation, making automated parsing complex.</p>

<p><strong>High item volume and potential for ambiguous product descriptions</strong><br>
Large quantities of items with unclear or incomplete specifications require intelligent interpretation.</p>

<p><strong>Massive catalog of internal products requiring intelligent filtering</strong><br>
The extensive product database needs efficient search and filtering mechanisms.</p>

<p><strong>Frequent mismatches between tender items and catalog availability</strong><br>
Many tender requirements don't align perfectly with available catalog items.</p>

<p>Moreover, Arthur Weber's product database is vast. Ensuring that each extracted item description is complete with all necessary specifications to match the correct database entry is a demanding task.</p>

<p>The AI solution developed by the team helps address these issues by increasing speed, improving accuracy, and establishing a scalable foundation for future automation.</p>
  <h2>🛠️ Technologies</h2>
  <table>
    <tr>
      <td align="center"><b>Programming</b></td>
      <td align="center"><b>Libraries</b></td>
      <td align="center"><b>Tools & Platforms</b></td>
    </tr>
    <tr>
      <td align="left" valign="top">
        <ul style="margin-top: 0; padding-left: 20px; text-align: left;">
          <li>Python 3.11</li>
        </ul>
      </td>
      <td align="left" valign="top">
        <ul style="margin-top: 0; padding-left: 20px; text-align: left;">
          <li>pdfplumber</li>
          <li>re (regular expressions)</li>
          <li>pandas</li>
          <li>json</li>
          <li>openai</li>
          <li>dotenv</li>
        </ul>
      </td>
      <td align="left" valign="top">
        <ul style="margin-top: 0; padding-left: 20px; text-align: left;">
          <li>Jupyter Notebook</li>
          <li>OpenAI API (GPT-4o-mini, GPT-4-turbo)</li>
        </ul>
      </td>
    </tr>
  </table>
</div>

<div>
  <h2>📜 Methodology</h2>
  <ul>
    <li><strong>PDF Text Extraction</strong>: Using pdfplumber to extract raw text from construction documents</li>
    <li><strong>Text Preprocessing</strong>: 
      <ul>
        <li>Cleaning text lines by removing unwanted characters and whitespace</li>
        <li>Identifying section headers based on predefined NPK section names</li>
        <li>Breaking documents into chunks by section</li>
        <li>Filtering for sections relevant to specific contractors</li>
        <li>Further splitting large sections into smaller, subsection chunks</li>
      </ul>
    </li>
    <li><strong>LLM-Based Information Extraction</strong>:
      <ul>
        <li>Parsing preprocessed text chunks</li>
        <li>Identifying construction items being ordered</li>
        <li>Extracting quantities, units, position numbers and metadata</li>
        <li>Returning structured JSON data</li>
      </ul>
    </li>
    <li><strong>Data Consolidation</strong>: Transforming extracted information into structured pandas DataFrames</li>
    <li><strong>Data Export</strong>: Exporting to CSV for further analysis</li>
  </ul>
</div>

<div>
  <h2>🔑 Key Features</h2>
  <ul>
    <li><strong>Sectional Processing</strong>: Identifies and filters specific sections of construction documents</li>
    <li><strong>Sophisticated Chunking Logic</strong>: Breaks down documents in ways that preserve context for the LLM</li>
    <li><strong>Detailed LLM Prompting</strong>: Carefully crafted prompts that explain construction document structure</li>
    <li><strong>Error Handling</strong>: Graceful handling of JSON parsing errors and API issues</li>
    <li><strong>Flexible Extraction</strong>: Works with different document formats and section types</li>
    <li><strong>Batch Processing</strong>: Processes multiple documents and combines results</li>
  </ul>
</div>
<div>
  <h2><img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Clipboard.png" alt="Presentation Icon" width="32" height="32" style="vertical-align: -0.25em;"> Project presentation slides</h2>
  <ul>
    <li><a href="https://guillermoibanez.github.io/Project-AI_Automation/AI_offer_Automation.pdf">Click here to check out the Project presentation slides.</a> </li>
  </ul>
</div>
<div>
  <h2><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python Icon" width="32" height="32" style="vertical-align: -0.25em;"> Project Code</h2>
  <ul>
    <li><a href="gpt_4o_mini_extraction.ipynb">Click here to view the extraction code</a>. This notebook contains the implementation for PDF extraction and LLM-based data structuring.</li>
  </ul>
</div>
<div align="center">
  <p>Last updated: May 2025.</p>
</div>
