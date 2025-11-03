# n8n Workflow: AI-Generated Notion Notes

![Workflow Preview](https://media.licdn.com/dms/image/v2/D4E22AQHYoRGCe_jeJw/feedshare-shrink_2048_1536/B4EZpIZEoMHUAw-/0/1762151124418?e=1763596800&v=beta&t=yACTdb8fBStqgCgItrWdBm4itCs5siXyIxMm4lGva5E)

This repository contains an n8n workflow that automates the generation of detailed, markdown-formatted notes for Notion using Google Generative AI. Given a topic, the workflow produces a structured note with a title and rich content, optimized for quick import into Notion.

---

## Features

- Uses Google Generative AI to create high-quality, human-like note content.
- Includes JSON schema validation to ensure structured and consistent output.
- Easily customizable prompt and schema for different note styles or topics.
- Handles errors gracefully with configurable 'On Error' settings in n8n.

---

## Getting Started

### Prerequisites

- An active n8n installation (self-hosted or cloud).
- Google Generative AI API credentials.
- Basic familiarity with n8n workflows and nodes.

### Installation

 **Import Workflow:**

   - Download the workflow JSON file from this repository.
   - In your n8n editor, click on “Import” and upload the workflow file.

 **Configure Credentials:**

   - Add your Google Generative AI API key in n8n’s Credentials section.
   - Edit the AI Agent node to use these credentials.

 **Customize Prompt (Optional):**

   - Open the AI Agent node.
   - Modify the prompt text if you want to adjust the note style or length.

     ```

 **Run Your Workflow:**

   - Trigger the workflow with a topic input.
   - Verify the output includes both a title and formatted markdown note content.

---

## Usage

This workflow is ideal for:

- Automating note creation from topics for personal or team knowledge bases.
- Summarizing research papers, articles, or meetings into Notion.
- Quickly generating structured documents with minimal manual effort.

You can extend the workflow by integrating with other tools or triggers (e.g., RSS feeds, form inputs).

---

## Troubleshooting

- **Output Format Errors:** If the model output doesn’t match the expected structure, set the root workflow node’s ‘On Error’ parameter to ‘Continue’ to avoid execution stops.
- **API Errors:** Double-check API key validity and quota limits.
- **Missing Content:** Ensure your prompt explicitly requests both title and note content in the desired JSON format.

---


## License

This project is licensed under the MIT License.

---