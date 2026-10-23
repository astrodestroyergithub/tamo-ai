# TamoAI — Global Top 500 AI Models Comparator, Live Benchmarks & Intelligence Hub

## 330-Character Non-Technical Platform Description
> **TamoAI is the ultimate all-in-one website to discover, compare, and test the world's top 500 AI models in real time. Filter models by price, speed, reasoning, and safety, chat with our unified TamoAI assistant, read full daily AI & India tech news, explore corporate tools, and download fresh AI keyword data—in 7 languages.** *(328 characters)*

## 1. Platform Overview & Inspiration
**TamoAI** is a responsive, high-density web application built for direct deployment on **Netlify**. It synthesizes the best capabilities of industry-leading LLM comparison platforms:
- **Vellum LLM Leaderboard** (`vellum.ai/llm-leaderboard`)
- **Stob.ai Model Comparison** (`stob.ai/ai-model-comparison`)
- **LiveBench Contamination-Free Evals** (`livebench.ai`)
- **BenchLM Pairwise Comparisons** (`benchlm.ai/compare`)
- **OpenRouter Multi-Provider Pricing & Routing** (`openrouter.ai/compare`)
- **Artificial Analysis Speed & Latency Telemetry** (`artificialanalysis.ai/leaderboards/models`)

## 2. Complete Feature Matrix & How to Use Every Section

| Section / Module | Key Capabilities | How to Use |
| :--- | :--- | :--- |
| **1. Top 500 AI Models Leaderboard** | Tracks 500 frontier & open-weight models across **Price ($/1M)**, **Reasoning (%)**, **Power Index**, **Weights**, **Status**, **Fair Play**, **Aggressiveness**, **Morality**, **MMLU-Pro**, **GPQA**, **HumanEval**, **SWE-Bench**, and **Speed (tok/s)**. | Use the 9 interactive sliders and dropdowns to filter all 500 models in real time. Click any column header to sort ascending/descending, or click `+ Compare` to send models to the Comparator. |
| **2. AI Model Comparator** | Side-by-side radar charts, grouped benchmark bar charts, and a 18-row technical comparison matrix for up to 6 models simultaneously. | Switch to **AI Model Comparator** in the top navigation bar. Remove or swap models at any time and inspect radar overlays. |
| **3. TamoAI Meta-Core (`TamoAI-Omni-Ultra v4`)** | Unified AI assistant combining formal CoT verification (`o3`/`DeepSeek-R1`), code synthesis (`Claude-3.7`), 2M multimodal context (`Gemini-2.5-Pro`), and 22-language Indic fluency (`Krutrim-2`/`Sarvam-2B`). | Open **TamoAI Meta-Core**, select a routing policy (Ensemble Top-5, Formal Proof, Sub-200ms Edge, or Sovereign Indic), and click a preset prompt or type your own query. |
| **4. Inference & Playground** | Dual-model sandbox allowing users to test any two models from the Top 500 side-by-side with custom temperature controls. | Open **Inference & Playground**, pick Model Slot A and Model Slot B, adjust temperature, and click **Run Dual Inference**. |
| **5. AI News & Blog (100% Thumbnail Verified)** | Displays curated and live-synced AI dispatches in **Grid**, **Tiles**, or **Table** layouts. Never renders any item without a thumbnail. | Filter by **Last 1 Hour**, **Last 1 Day**, **Last 1 Month**, or **Last 1 Year**. Click any card to open the **Full Story Reader Modal** (unabridged article + architecture diagrams + direct link to the original source). Click 👍 Like, 👎 Dislike, or 🔖 Bookmark on any card. |
| **6. India AI Sovereign Hub** | Dedicated tracker for Indian AI models (`Krutrim-2-70B`, `Sarvam-2B`, `BharatGen-108B`, `Bhashini 22-Language Grid`, `AI4Bharat`). | Open **India AI Sovereign Hub**, filter by recency (Last Hour, Last Day, Last Month), and click any capsule to read the full unabridged technical story. |
| **7. Corporate Tech Stack** | Contrasts legacy corporate engineering (3 years ago: multi-sprint manual coding) against modern autonomous workflows (2-hour feature delivery via MCP, Cursor, Devin, Braintrust CI evals, and Confidential GPU Enclaves). | Open **Corporate Tech Stack** to inspect side-by-side Legacy vs. Modern workflow cards. Rotates automatically every 24–48 hours or on clicking **Rotate Corporate Feed (+48h)**. |
| **8. Strange & Uncanny AI Vault** | Investigates rare, lesser-known AI paradigms: biological cortical organoid wetware (`DishBrain`), emergent steganographic CoT ciphers, and 1.58-bit room-temperature photonic chips. | Open **Strange & Uncanny AI** to read full technical dossiers. Rotates completely every 1–2 days. |
| **9. Token & Keyword CSV Scraper** | Captures 1,000 to 5,000 high-velocity AI keywords, TF-IDF frequencies, and training prompts from Google, YouTube, arXiv, and HuggingFace. | Open **Token & CSV Scraper**, enter your target query, choose token volume (up to 5,000 rows), click **Trigger Live Scrape**, and click **Download Full Scraped CSV Dataset**. You can also run `python3 backend/tamoai_scraper_engine.py` from the terminal. |
| **10. 18+ Specialized Arenas & Labs** | Integrates **LLM Leaderboard**, **Image Arena**, **Video Arena**, **AI Agents**, **Evaluations**, **MicroEvals**, **Model Recommender**, **Data Playground**, **Image Lab**, **Analysis**, **Products**, **Methodology**, **Articles**, **FAQs**, **Community**, and **Resources**. | Open **Arenas & Labs**, use the **Smart Model Recommender** to compute the Pareto-optimal model for your budget, or click any of the 16 module cards to execute live telemetry diagnostics. |
| **11. 7-Language Instant Localization** | Translates visible UI labels, navigation, headers, and filters across **English, Hindi, Bengali, French, German, Spanish, and Chinese**. | Use the language dropdown in either the top header or the bottom footer to switch languages immediately. |
| **12. Premium Tiers & Checkout** | Supports **$20, $150, $580, and $2450 / month** tiers with full card checkout validation to unlock Discreet AI Trends & Illustrations. | Click **Upgrade to Premium** in the top header, select your tier, complete the cardholder form, and unlock the discreet vault. |

## 3. Dynamic 24–48 Hour Feed Rotation Architecture
To guarantee that visitors never see stale static content day after day:
1. **Epoch-Seeded Rotation (`getCurrentEpochSeed`)**: All feeds calculate a deterministic 36-to-48-hour time epoch from the system clock and rotate feed items, cycle badges, and rankings automatically.
2. **Interactive Time-Travel Simulator**: Click **Simulate +48h Feed Shift** in the top bar at any time to immediately preview how the entire platform transforms 2 days into the future.
3. **Live Open-Source API Sync (`syncLiveOpenSourceAPIs`)**: Connects directly to the **OpenRouter Models API** (`https://openrouter.ai/api/v1/models`) and **HackerNews Algolia API** (`https://hn.algolia.com/api/v1/search_by_date`) in the browser, while the Python backend script (`backend/tamoai_scraper_engine.py`) pulls from **arXiv API**, **HuggingFace Hub API**, and **OpenRouter**.

## 4. Deploying to Netlify
### Method A: Instant Drag-and-Drop (Netlify Drop)
1. Download `tamoai_netlify_bundle.zip` and extract it, or drag the ZIP/folder directly onto [app.netlify.com/drop](https://app.netlify.com/drop).
2. Netlify will automatically serve `index.html`, `css/styles.css`, `js/app.js`, `assets/`, and the serverless function in `netlify/functions/live_feed.py` using `netlify.toml`.

### Method B: CLI or Git Deployment
```bash
# 1. Run the Python scraper locally to refresh the 5,000-token CSV dataset
python3 backend/tamoai_scraper_engine.py --query "Frontier LLMs, MoE, India AI" --tokens 5000 --output sample_scraped_ai_keywords_500.csv

# 2. Deploy via Netlify CLI
netlify deploy --prod --dir=.
```
