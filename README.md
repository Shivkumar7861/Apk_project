# SANA (Shiv APK Network Analyzer)

**SANA** is a powerful, open-source APK analysis tool built with a focus on transparency, privacy, and intelligent threat detection. It allows developers, researchers, and users to inspect Android APK files before installation to detect potential security risks, misconfigurations, and malicious behavior.

## 🔍 Project Highlights

* ✨ **Frontend**: Built with **Next.js**, **Tailwind CSS**, and **Radix UI** for a responsive, modern interface
* 🧠 **AI-Powered Risk Detection**: Uses **Genkit** with **Google Gemini** to assess APK names and permission patterns for suspicious behavior
* 🛡️ **Static APK Analysis**: Extracts details from `AndroidManifest.xml` like permissions, SDK versions, components, and flags issues
* 📄 **Detailed Reporting**: Generates human-readable reports including SHA-256 hash, risk levels, and optional PDF export
* 🔐 **Privacy-First**: Designed for local or self-hosted deployment without sending data to the cloud

## 🚀 Features

* Upload `.apk` files via an intuitive UI
* Analyze manifest data: permissions, SDK targets, services, receivers
* Detect dangerous or excessive permission usage
* Leverage AI to identify behavioral red flags
* View risk summary and recommendations
* Download full JSON or PDF reports
* SHA-256 fingerprinting for integrity and tracking
* Export project as ZIP (excluding node\_modules and Git)

## 🛠️ Tech Stack

* **Frontend**: Next.js, Tailwind CSS, Radix UI
* **Backend**: Flask (Python)
* **AI**: Genkit + Google Gemini
* **APK Parsing**: XML, zipfile (Python), Androguard (optional)
* **Reporting**: JSON, jsPDF, Zod

## 📦 Project Structure

```bash
src/
├── ai/           # Genkit flows for Gemini-based risk analysis
├── app/          # UI layout, global CSS, routing
├── components/   # APK analyzer form, result cards, reusable UI
├── hooks/        # Toast notifications, mobile detection
├── lib/          # Utility functions (e.g., class merging)
```

## 🧠 Use Cases

* Analyze APKs before installation
* Identify malware, spyware, or over-permissioned apps
* Generate reports for security audits
* Learn about Android app security internals

## 📥 Installation (Dev)

```bash
# 1. Backend
cd backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python app.py

# 2. Frontend
cd ../project
npm install
npm run dev
```

## 🙋‍♂️ Author

Built by **Shivcharan Ahirwar** under the ISEA internship program at **C-DAC**.

## 📜 License

This project is open-source under the [MIT License](LICENSE).
