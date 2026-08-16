\# 🤖 JARVIS — Personal AI Desktop Assistant



> A voice-controlled personal AI assistant powered by Google's Gemini Live API, designed to interact with your computer, understand natural language commands, use tools, process visual information, and automate everyday desktop tasks.



\---



\## 🚀 Overview



JARVIS is a personal AI desktop assistant built with Python and Google's Gemini Live API.



It combines \*\*real-time voice interaction, AI reasoning, computer automation, browser control, vision capabilities, memory, and a local wake-word system\*\* into a single assistant.



Instead of continuously sending microphone audio to the AI, JARVIS uses a local wake-word detector and only activates the AI voice pipeline when the user says:



> 🎙️ \*\*"Hey JARVIS"\*\*



After completing a command, JARVIS returns to wake-word mode and waits for the next activation.



\---



\## ✨ Features



\### 🎙️ Voice Interaction

\- Real-time microphone input

\- Gemini Live voice interaction

\- Natural conversational responses

\- Local wake-word detection

\- Wake-word controlled microphone activation

\- Returns to sleep mode after each command



\### 🧠 AI Intelligence

\- Powered by Google's Gemini Live API

\- Natural-language understanding

\- Context-aware conversations

\- Tool/function calling

\- Memory system for important user preferences and information

\- Proactive assistance capabilities



\### 🖥️ Computer Control

JARVIS can interact with the Windows desktop and perform tasks such as:



\- Opening and closing applications

\- Controlling volume

\- Adjusting brightness

\- Managing windows

\- Keyboard shortcuts

\- System operations

\- Desktop organization

\- File and folder operations



\### 🌐 Browser Automation

JARVIS can interact with web browsers to:



\- Open websites

\- Search the web

\- Navigate pages

\- Click elements

\- Enter text

\- Fill forms

\- Perform browser-based tasks



\### 👁️ Vision

JARVIS can process visual information using:



\- Screen capture

\- Webcam input

\- Image analysis

\- Screen understanding

\- Visual question answering



Example:



> "Hey JARVIS, what's on my screen?"



\### 🧠 Memory

JARVIS includes a memory system that can store useful information such as:



\- User preferences

\- Important personal context

\- Project information

\- Frequently used information



This allows JARVIS to provide more personalized responses over time.



\### 📱 Remote Interaction

The project also includes support for remote/phone interaction, allowing commands and microphone input to be relayed to the desktop assistant.



\### ⚙️ Windows Startup

JARVIS can be configured to automatically start when Windows starts using Windows Task Scheduler.



\---



\# 🏗️ Architecture



```text

&#x20;                   ┌──────────────────────┐

&#x20;                   │      User Voice      │

&#x20;                   └──────────┬───────────┘

&#x20;                              │

&#x20;                              ▼

&#x20;                   ┌──────────────────────┐

&#x20;                   │   Local Wake Word    │

&#x20;                   │    "Hey JARVIS"      │

&#x20;                   └──────────┬───────────┘

&#x20;                              │

&#x20;                        Wake Detected

&#x20;                              │

&#x20;                              ▼

&#x20;                   ┌──────────────────────┐

&#x20;                   │    Microphone Input  │

&#x20;                   └──────────┬───────────┘

&#x20;                              │

&#x20;                              ▼

&#x20;                   ┌──────────────────────┐

&#x20;                   │     Gemini Live      │

&#x20;                   │        API           │

&#x20;                   └──────────┬───────────┘

&#x20;                              │

&#x20;                              ▼

&#x20;                   ┌──────────────────────┐

&#x20;                   │     AI Reasoning     │

&#x20;                   └──────────┬───────────┘

&#x20;                              │

&#x20;             ┌────────────────┼────────────────┐

&#x20;             │                │                │

&#x20;             ▼                ▼                ▼

&#x20;      ┌────────────┐   ┌────────────┐   ┌────────────┐

&#x20;      │   Desktop  │   │  Browser   │   │   Vision   │

&#x20;      │   Control  │   │   Control  │   │   System   │

&#x20;      └────────────┘   └────────────┘   └────────────┘

&#x20;             │                │                │

&#x20;             └────────────────┼────────────────┘

&#x20;                              │

&#x20;                              ▼

&#x20;                   ┌──────────────────────┐

&#x20;                   │   Gemini Response    │

&#x20;                   │    Voice Output      │

&#x20;                   └──────────┬───────────┘

&#x20;                              │

&#x20;                              ▼

&#x20;                   ┌──────────────────────┐

&#x20;                   │     Sleep / Wait     │

&#x20;                   │   "Hey JARVIS..."    │

&#x20;                   └──────────────────────┘

