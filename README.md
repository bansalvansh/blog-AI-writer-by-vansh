# AI Blog Generator Using Notion + ChatGPT

A blog automation tool built using Notion, OpenAI GPT-4 API, and automation scripts. Originally inspired by gr8monk3ys/blog-AI and customized for my workflow.

## Features
- Auto-generate blogs from Notion content prompts
- GPT-based long-form content creation
- SEO-friendly formatting
- Easily pluggable into Notion or Webflow blog systems

## Quick Setup

### Prerequisites
- Python 3.12 or later
- Node.js 14.x or later
- OpenAI API key (get one at https://platform.openai.com/)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/bansalvansh/blog-AI-writer-by-vansh.git
   cd blog-AI-writer-by-vansh
   ```

2. **Set up environment variables:**
   ```bash
   cp .env.example .env
   ```
   Then edit the `.env` file and replace `### YOUR KEY HERE` with your actual API keys:
   ```
   OPENAI_API_KEY=sk-your-actual-openai-api-key-here
   ANTHROPIC_API_KEY=your-anthropic-key-here  # Optional
   SERP_API_KEY=your-serp-api-key-here       # Optional for web research
   SEC_API_API_KEY=your-sec-api-key-here     # Optional
   ```

3. **Install backend dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Install frontend dependencies:**
   ```bash
   cd frontend
   npm install
   cd ..
   ```

### Running the Application

1. **Start the backend server:**
   ```bash
   python server.py
   ```
   The backend will be available at http://localhost:8000

2. **Start the frontend (in a new terminal):**
   ```bash
   cd frontend
   npm run dev
   ```
   The frontend will be available at http://localhost:3000

3. **Open your browser and navigate to http://localhost:3000**

## Troubleshooting

If you see "Failed to generate content" errors:
- Make sure you've set a valid OpenAI API key in your `.env` file
- Ensure your OpenAI account has billing set up and credits available
- Check the `troubleshooting.md` file for detailed troubleshooting steps

## Testing

Run the test suite to verify everything is working:
```bash
python run_tests.py
```
