# Automated Marketing Content Generator

# Project Overview

This project is an Automated Marketing Content Generator built using n8n, designed to generate creative marketing content automatically for a selected brand (Nike in this example). The workflow integrates several APIs and automation steps to produce social media posts, content plans, and engagement data with minimal manual effort.

# How It Works
	•	The workflow is triggered manually via the Manual Trigger node.
	•	It sends a custom JSON query about the brand Nike to a RapidAPI HTTP endpoint to fetch detailed brand information.
	•	The fetched data is processed by a LangChain LLM node using OpenAI’s GPT-4o model to:
	•	Create a concise brand overview.
	•	Generate 5 creative social media post ideas with captions.
	•	Develop a one-week Instagram content plan.
	•	List 10 trending hashtags relevant to Nike.
	•	A JavaScript Code node formats the output to fit the requirements of multiple platforms (Facebook, Instagram, Twitter).
	•	The formatted content is sent via Telegram API to deliver the results directly to a chat.
	•	Additionally, some data is saved into a Google Sheets spreadsheet for record-keeping.
	•	Other HTTP requests are used for data interactions or to trigger further automation steps.

# Tools and Technologies Used
	•	n8n for workflow automation.
	•	Manual Trigger node to start the process.
	•	HTTP Request node to call external APIs (RapidAPI for brand data, Telegram API for messaging).
	•	LangChain Chain LLM node integrated with OpenAI GPT-4o language model for content generation.
	•	Code (JavaScript) nodes for customizing and formatting data.
	•	Google Sheets node to create and update spreadsheets with generated data.

# Final Outputs
	•	Automatically generated creative social media posts tailored for Facebook, Instagram, and Twitter.
	•	A structured content plan for Instagram.
	•	Delivered content directly to Telegram.
	•	Organized storage of data and metrics in Google Sheets.

 
