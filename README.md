# 🦴 Fracto - AI-Powered Fracture Analysis Platform

Fracto is a cutting-edge web application that leverages artificial intelligence to analyze radiographic images for bone fractures. Built with Next.js and powered by OpenAI's GPT-4 Vision, Fracto provides detailed medical assessments of X-ray images to assist in orthopedic evaluation.

## ✨ Features

- **🔍 AI-Powered Analysis**: Advanced computer vision using OpenAI GPT-4o for accurate fracture detection
- **📋 Clinical Context Integration**: Optional clinical notes input to enhance analysis accuracy
- **🏥 Medical-Grade Interface**: Professional healthcare-focused UI with Material 3 design principles
- **📊 Structured Reports**: Comprehensive analysis including fracture type, location, severity, and treatment recommendations
- **⚡ Real-time Processing**: Fast image upload and analysis with live status updates
- **🔒 Secure**: Built with modern security practices for handling medical data

## 🏥 Medical Capabilities

Fracto analyzes radiographic images and provides structured assessments including:

- **Image Quality Assessment**: Evaluation of radiograph clarity and diagnostic quality
- **Fracture Detection**: Identification of present or absent fractures
- **Fracture Classification**: Type classification (transverse, oblique, spiral, comminuted, etc.)
- **Anatomical Mapping**: Precise bone and anatomical region identification
- **Severity Evaluation**: Assessment of displacement, angulation, and comminution
- **Clinical Recommendations**: Treatment suggestions and management approaches
- **Prognosis**: Recovery timeline estimates and healing considerations

## 🚀 Technology Stack

- **Frontend**: Next.js 15, React 19, TypeScript
- **Styling**: Tailwind CSS with custom healthcare color palette
- **AI Processing**: OpenAI GPT-4o Vision API
- **Deployment**: Vercel-ready configuration

## ⚙️ Setup & Installation

### Prerequisites

- Node.js 18+ 
- OpenAI API key with GPT-4 Vision access
- npm, yarn, pnpm, or bun

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd fracto
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Configure environment variables**
   ```bash
   cp .env.example .env.local
   ```
   
   Add your OpenAI API key to `.env.local`:
   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   ```

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Open the application**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 📖 Usage

1. **Upload Image**: Click the upload area to select a radiographic image (PNG, JPG, or DICOM)
2. **Add Clinical Context** (Optional): Provide patient history, symptoms, or mechanism of injury
3. **Analyze**: Click "Analyze Fracture" to process the image
4. **Review Results**: Examine the comprehensive AI-generated analysis report

## 🔧 API Endpoints

### `POST /api/analyze-fracture`

Analyzes uploaded radiographic images for fractures.

**Request Body:**
```json
{
  "imageData": "data:image/jpeg;base64,/9j/4AAQ...", 
  "clinicalNotes": "Optional clinical context"
}
```

**Response:**
```json
{
  "analysis": "Detailed fracture analysis...",
  "timestamp": "2025-07-04T12:00:00.000Z",
  "model": "gpt-4o"
}
```

## ⚠️ Medical Disclaimer

**IMPORTANT**: Fracto is designed for educational and demonstration purposes only. This application:

- Should NOT be used for actual medical diagnosis or treatment decisions
- Does not replace professional medical evaluation
- Requires consultation with qualified healthcare professionals for proper medical care
- Is not FDA approved or medically certified

Always consult with licensed medical professionals for actual patient care.

## 🏗️ Project Structure

```
fracto/
├── src/
│   ├── app/
│   │   ├── api/analyze-fracture/
│   │   │   └── route.ts          # AI analysis API endpoint
│   │   ├── globals.css           # Global styles
│   │   ├── layout.tsx            # Root layout
│   │   └── page.tsx              # Main application interface
│   └── ...
├── public/                       # Static assets
├── .env.example                  # Environment variables template
└── README.md
```

## 🔮 Future Enhancements

- [ ] DICOM file format support
- [ ] Multi-view X-ray analysis
- [ ] Integration with medical imaging systems
- [ ] Advanced fracture classification algorithms
- [ ] Report export functionality
- [ ] User authentication and patient management
- [ ] Integration with electronic health records (EHR)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.

## 📄 License

This project is for educational and demonstration purposes. See the LICENSE file for details.

---

Built with ❤️ for advancing medical technology through AI
