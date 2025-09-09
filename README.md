# Image Processing Application

This project provides an interactive web-based application for **image generation and inpainting** using state-of-the-art diffusion models. Built with **Streamlit** and powered by **Hugging Face Diffusers**, the app enables users to upload images, mask regions for inpainting, and generate/edit images using natural-language prompts.

## Table of Contents

- [Introduction](#introduction)  
- [Problem Definition](#problem-definition)  
- [Features](#features)  
- [Installation](#installation)  
  - [System requirements](#system-requirements)  
  - [Clone & virtual environment](#clone--virtual-environment)  
  - [Install PyTorch (GPU/CPU)](#install-pytorch-gpucpu)  
  - [Install Python dependencies](#install-python-dependencies)  
  - [Optional: LocalTunnel (share publicly)](#optional-localtunnel-share-publicly)  
  - [Hugging Face credentials](#hugging-face-credentials)  
- [Usage](#usage)  
  - [Run locally](#run-locally)  
  - [Run with a tunnel (optional)](#run-with-a-tunnel-optional)  
- [References](#references)  
- [License](#license)

## Introduction

Recent advances in generative models make realistic image editing accessible through simple text instructions. This application wraps model inference into a small Streamlit interface so users can experiment with prompt-driven image generation and inpainting without complex setup.

## Problem Definition

Manual image editing is time-consuming and often requires skill with graphical tools. The goal of this project is to provide an **easy-to-use interface** that allows users to:
- Generate images from text prompts.
- Edit parts of existing images by masking (inpainting).
- Quickly iterate on prompts and settings to produce desired outputs.

## Features

- **Text-to-Image Generation** using diffusion models.
- **Inpainting**: mask a region of an input image and fill it according to a prompt.
- **Streamlit UI**: lightweight interactive frontend for experimentation.
- **GPU support**: uses PyTorch/CUDA when available for faster inference.
- **Simple deployment**: runs locally or can be exposed using tools like `localtunnel` or `ngrok`.

## Installation

### System requirements
- Python 3.8+ (3.9 or 3.10 recommended).
- Optional GPU with CUDA (for faster inference). The app runs on CPU if no GPU is present (slower).
- `git`, `node`/`npm` (optional, for LocalTunnel via `npx`).

### Clone & virtual environment
```bash
git clone https://github.com/your-username/Image-Processing-Application.git
cd Image-Processing-Application

# Create & activate venv (Linux / macOS)
python -m venv venv
source venv/bin/activate

# Windows (PowerShell)
python -m venv venv
venv\Scripts\Activate.ps1
