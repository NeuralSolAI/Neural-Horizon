# Neural Horizon AI

## Overview

**$NRHZ - Neural Horizon AI**  
The Neural Horizon Twitter Bot is a TypeScript-based project designed to combine AI-generated visuals and social media automation. It generates Neural Horizon-themed artwork, futuristic waveform videos, and engaging Twitter content. The bot uses the AI16z framework to power its creative outputs and the Twitter API for seamless posting.

---

## Features

 - **Waveform Video Generation**: Converts Neural Horizon-themed text into dynamic waveform videos.
- **Automated Daily Posting**: Posts multimedia content on Twitter with formatted captions.
- **Customizable Content**: Offers flexibility in prompts, themes, and styles.
- **Error Handling**: Includes error management for uninterrupted operation.

**by @NeuralHorizonAI**

---

## Setup

### 1. Clone the Repository

```bash
git clone [https://github.com/yourusername/neural-horizon-ai](https://github.com/NeuralSolAI/Neural-Horizon.git)
cd neural-horizon-ai
```
### 2. Install Dependencies

```bash
npm install
```
### 3. Configure API Keys
Update the .env file or set environment variables:
```bash
TWITTER_API_KEY=your_api_key
TWITTER_API_SECRET=your_api_secret
TWITTER_ACCESS_TOKEN=your_access_token
TWITTER_ACCESS_SECRET=your_access_secret
AI_API_KEY=your_ai_api_key
```

###  Usage
```bash
npm start
```
 

## Code Breakdown

### Agent Setup

The bot initializes an AI agent using the `createAgent` function from `@ai16z/eliza`. It is configured to generate text-to-waveform videos with a high creativity level.

### Waveform Video Generation

The `generateWaveformForText` function takes user-provided text and converts it into a dynamic waveform video. This process includes:
- **Text-to-Speech Conversion**: The input text is synthesized into audio.
- **Waveform Animation**: A futuristic waveform animation, styled to match the Neural Horizon theme, is generated and synchronized with the audio.

### Tweet Posting

The `postContentToTwitter` function formats and posts the multimedia content using the `sendTweet` API. Each post includes:
- The generated waveform video.
- A caption that provides context about the content and includes attribution details.

### Automation

The bot uses `setInterval` to schedule daily posts. The posting frequency can be adjusted by modifying the interval in the `setInterval` function.
"""


