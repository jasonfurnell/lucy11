# ElevenLabs AI Assistant Setup Guide

This guide will walk you through the process of setting up your ElevenLabs AI Assistant website from start to finish.

## 1. Create Your ElevenLabs Account

1. Go to [ElevenLabs](https://elevenlabs.io/sign-up) and create an account
2. Familiarize yourself with the dashboard

## 2. Create Your Conversational AI Agent

1. In the ElevenLabs dashboard, navigate to the **Conversational AI** section
2. Click **Create New Agent** or similar button
3. Choose a template or create a blank agent

## 3. Configure Your Agent

### Basic Configuration
- **Name**: Give your agent a descriptive name
- **First Message**: Set the initial greeting message

### System Prompt
Configure the system prompt to define your agent's behavior:

```
You are a helpful assistant for [your company/service]. Your goal is to provide information about [topic/service] and assist users with their questions.

Key facts you know:
- [Fact 1]
- [Fact 2]
- [Fact 3]

When answering questions:
- Be helpful, concise, and friendly
- If you don't know the answer, say so and offer to connect them with a human
- Always maintain a [formal/casual/professional] tone

If users ask about pricing, inform them that [pricing information].
```

### Knowledge Base
Add relevant documents to help your agent answer questions:
- Upload PDFs, Word docs, or text files
- Add website URLs for the agent to reference
- Add FAQs in text format

### Voice Selection
Choose a voice that matches your brand:
- Browse the available voices
- Test different options
- Select one that fits your brand identity

### Evaluation Criteria (Optional)
Set up criteria to evaluate conversation success:
- Define what constitutes a successful interaction
- Specify data points to collect from conversations

## 4. Test Your Agent

1. Use the test functionality in the ElevenLabs dashboard
2. Try various questions and scenarios
3. Refine prompts and knowledge base as needed

## 5. Get Your Agent ID

1. From your agent's dashboard, look for the embed or integration section
2. Copy your unique **Agent ID**

## 6. Configure Your Website

1. Open the `index.html` file from this repository
2. Find the following line near the bottom:
   ```html
   <div id="elevenlabs-convai-widget" data-agent-id="YOUR_AGENT_ID_HERE"></div>
   ```
3. Replace `YOUR_AGENT_ID_HERE` with your actual Agent ID

## 7. Customize Your Website (Optional)

- Update the text content in `index.html`
- Modify styles in `styles.css`
- Add your own logo and images
- Update contact information

## 8. Deploy to GitHub Pages

1. Push your changes to your GitHub repository
2. Go to your repository settings
3. Navigate to the Pages section
4. Select the branch to deploy (usually `main`)
5. Save your settings
6. Wait for GitHub to build and deploy your site (usually takes 1-2 minutes)
7. Access your site at `https://[your-username].github.io/[repository-name]/`

## 9. Test on Live Site

1. Visit your deployed website
2. Test the AI assistant widget
3. Make any necessary adjustments

## Troubleshooting

### Widget Not Appearing
- Verify your Agent ID is correct
- Check browser console for errors
- Ensure the ElevenLabs script is loading properly

### Audio Issues
- Make sure microphone permissions are granted
- Check if your browser supports the required features
- Try using Chrome or Edge for best compatibility

### Response Quality Issues
- Review and enhance your knowledge base
- Refine your system prompt
- Add more specific instructions to guide responses

## Next Steps

- Monitor conversations in your ElevenLabs dashboard
- Gather user feedback
- Regularly update your knowledge base
- Refine prompts based on common questions
