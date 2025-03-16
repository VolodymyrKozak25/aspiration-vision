# Aspiration Vision

A cross-platform desktop application that continuously monitors your screen, recognizes text using OCR, translates it using external translation APIs, and overlays the translated text in real time. Built with Rust for both the UI and backend and Python for OCR, the app is designed to be minimal, lightweight, and run in the background on both Windows and Linux.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Technology Stack](#technology-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Development](#development)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Overview

Aspiration Vision (AV) is a utility tool aimed at helping users overcome language barriers by translating text on their screen on the fly.

## Features

- **Real-Time Screen Monitoring:** Continuously monitors the screen for text changes with debouncing to avoid excessive processing.
- **OCR Integration:** Uses Tesseract (pytesseract) for efficient text recognition.
- **Translation API Integration:** Connects to translation APIs (currently planned DeepL and Google Translate) using Rust's HTTP libraries.
- **Overlay Display:** Displays translated text over the original content with customizable font.
- **Minimal UI & Background Mode:** Operates with minimal on-screen footprint and runs in the background.

## Architecture

The application is built using a modular architecture:

- **User Interface:** Developing using Rust GUI framework (Iced).
- **OCR Module:** Integrates Tesseract OCR to capture on-screen text.
- **Translation Module:** Uses Rust’s `reqwest` crate to interact with external translation APIs.
- **Overlay Renderer:** Renders the translated text in an always-on-top window.
- **Background Service:** Runs continuously, monitoring the screen and processing updates.

A detailed system architecture diagram is available in the project wiki (soon).

## Technology Stack

- **Programming Languages:** Rust+Python
- **GUI Framework:** [Iced](https://github.com/hecrj/iced)
- **HTTP Client:** [reqwest](https://github.com/seanmonstar/reqwest)
- **OCR Integration:** [pytesseract](https://github.com/h/pytesseract)
- **Build & CI/CD:** GitHub Actions for continuous integration and deployment

## Installation
- **Will be available later(TODO)**
- 
### Prerequisites

- [Rust](https://www.rust-lang.org/tools/install) (latest stable version)
- Tesseract OCR installed on your system (for OCR functionality)
- An API key for your chosen translation service (DeepL or Google Translate)

### Building the Project

Clone the repository:

You can clone it as any other repository, but you probably don't want to, for now.
