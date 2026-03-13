# College AI Assistant (YMN GPT)

An intelligent, PWA-ready web application designed to serve as a smart assistant for college students, faculty, and visitors. It provides instant answers to queries about courses, admissions, fees, and campus life using a locally stored knowledge base and the powerful Groq API.

## 🚀 How It Works

1.  **Knowledge Base**: The app pre-loads information from text files located in the `clg_info/` directory. These files contain details about faculty, fees, general information, and more.
2.  **Local Storage**: Extracted text from these documents is stored locally in your browser using **IndexedDB**. This ensures fast access and privacy.
3.  **Semantic Search**: When you ask a question, the app performs a keyword-based search (with synonym expansion) across the local documents to find the most relevant context.
4.  **Web Scraping (Fallback)**: If the information isn't found locally, the app can optionally scrape the configured college website for real-time information.
5.  **AI Processing**: The gathered context is sent to the **Groq API** (using models like Llama 3) to generate a professional, helpful, and accurate response.
6.  **PWA Support**: The app can be installed on your mobile or desktop device for a native-like experience.

## 🏁 How to Start

1.  **Login to Admin Panel**: Open the app and click the **Gear Icon** (top right) or go to `your-url.com/#admin`. Enter the admin password (default is `admin123`).
2.  **Provide Groq API Key**: In the Admin Dashboard, paste your **Groq API Key** into the required field and click **"Save Configuration"**.
3.  **Add Knowledge Base**: Upload your college's text, PDF, or DOCX files in the **"Knowledge Base"** section. The app will automatically process and store them locally.
4.  **Start Chatting**: Go back to the chat view and start asking questions!

## 🔑 How to Generate a Groq API Key

To use this assistant, you need a Groq API key. Follow these steps:

1.  **Go to the Groq Console**: Visit [https://console.groq.com/](https://console.groq.com/).
2.  **Sign Up / Log In**: Create an account or sign in using your existing credentials.
3.  **Navigate to API Keys**: On the left sidebar, click on the **"API Keys"** section.
4.  **Create a New Key**:
    *   Click the **"Create API Key"** button.
    *   Give your key a name (e.g., "CollegeGPT").
    *   **Copy the key immediately!** You won't be able to see it again for security reasons.
5.  **Configure the App**:
    *   Open the College AI Assistant web page.
    *   Click the **Gear Icon** (Admin Panel) in the top right.
    *   Enter the admin password (default is `admin123`).
    *   Paste your key into the **"Groq API Key"** field and click **"Save Configuration"**.

## 🌟 Why This is Useful

*   **Instant Information**: No more digging through complex websites or PDF handbooks. Get answers to "How much is the B.Tech fee?" or "Who is the HOD of Computer Science?" in seconds.
*   **24/7 Availability**: The assistant is always online to help prospective students and parents, even outside college office hours.
*   **User-Friendly**: Provides interactive suggestion bubbles to help users discover what they can ask.
*   **Privacy-Focused**: Your documents and API keys are stored locally in your browser's database, not on a central server.
*   **Customizable**: Administrators can easily update the knowledge base by uploading new PDF, TXT, or DOCX files directly through the dashboard.

## 🛠️ Setup & Deployment

Since this is a single-file application with local storage:
1.  Clone this repository.
2.  Host it on **GitHub Pages**, **Vercel**, or use a local server (like VS Code's "Live Server").
3.  Ensure the `clg_info/` folder is in the same directory as `index.html`.
4.  Access the admin panel at `your-url.com/#admin` to configure your API key.

---
*Built with ❤️ for better campus accessibility.*
