# 🧬 PediGen AI

**AI-Powered Genetic Pedigree Chart Generator**

[![License](https://img.shields.io/badge/License-MIT%20with%20Academic%20Reservation-blue.svg)](LICENSE)

<p align="center">
  <img src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" alt="PediGen AI Banner" width="800"/>
</p>

PediGen AI transforms natural language descriptions of family medical history into standardized genetic pedigree charts. Simply describe a family's health history, and the AI generates a complete, interactive pedigree following clinical genetics conventions.

## ✨ Features

- **🤖 AI-Powered Generation**: Describe family history in plain text → get a structured pedigree
- **🏥 Clinical Genetics Standards**: Proper symbols for affected, carrier, deceased, and unaffected individuals
- **👥 Complex Relationships**: Support for consanguinity, twins (monozygotic/dizygotic), and multiple generations
- **🎯 Proband Marking**: Identify the index case/consultand
- **🏷️ Multiple Conditions**: Track multiple genetic conditions with color coding
- **💾 Save & Export**: Save pedigrees locally, export as JPEG or JSON
- **✏️ Interactive Editing**: Click to select and modify individuals
- **🔄 AI Refinement**: Provide feedback to refine generated pedigrees


## 🚀 Quick Start

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- A Gemini API key ([Get one here](https://makersuite.google.com/app/apikey))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/hipokrart/pedigen-ai.git
   cd pedigen-ai
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env.local
   ```
   Then edit `.env.local` and add your Gemini API key:
   ```
   GEMINI_API_KEY=your_api_key_here
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:5173`

## 📖 Usage

### Generating a Pedigree from Text

Enter a natural language description of the family history:

```
The proband is a 10-year-old boy affected with cystic fibrosis. 
His father (54) is a carrier, and his mother (52) is unaffected. 
He has a twin sister who is unaffected. The paternal grandfather 
is deceased, and the maternal uncle is also affected.
```

The AI will generate a complete pedigree with:
- All family members properly positioned
- Correct relationship lines
- Medical status symbols
- Twin connections

### Manual Editing

- Click any individual to select and edit their properties
- Add new family members through the sidebar
- Define custom conditions with color coding

### Exporting

- **Export Image**: Download the pedigree as a JPEG
- **Export JSON**: Download structured data for backup or further processing

## 🛠️ Tech Stack

- **Frontend**: React 19, TypeScript
- **Visualization**: D3.js
- **AI**: Google Gemini API
- **Build Tool**: Vite
- **Styling**: Tailwind CSS


## 🤝 Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

Please read the [LICENSE](LICENSE) regarding academic use and publications.

## 📄 License

This project is licensed under the **MIT License with Academic and Commercial Reservation** — see the [LICENSE](LICENSE) file for details.

**Important**: If you use this software in academic publications, please see our citation requirements and contact the authors.

## 📚 Citation

If you use PediGen AI in your research, please cite:

```bibtex
@software{pedigen_ai_2026,
  author = {[Efe Deniz SENGUN, Deniz AYDOGDU]},
  title = {PediGen AI: AI-Powered Genetic Pedigree Chart Generator},
  year = {2026},
  url = {https://github.com/hipokrart/pedigen-ai}
}
```


## 📧 Contact

For academic collaboration, commercial licensing, or questions:
- Email: [edsengun@gmail.com]
- GitHub Issues: [Open an issue](https://github.com/hipokrart/pedigen-ai/issues)

## 🙏 Acknowledgments

- Built with [Google Gemini](https://deepmind.google/technologies/gemini/)
- Pedigree standards based on [NSGC guidelines](https://www.nsgc.org/)
- D3.js visualization library

---

<p align="center">Made with ❤️ for the genetics community</p>
