# Email Tagging System

## Description

This Python project is an **Email Tagging System** that automatically tags emails in your Outlook inbox based on their subject and body content. It categorizes emails into tags such as "urgent", "important", "work", "time-sensitive", and more using regex patterns. The system also allows users to filter, view, and remove tags from emails through a simple graphical user interface (GUI) built with **Tkinter**.

## Features

- **Email Fetching**: Fetch emails from your Outlook inbox.
- **Auto Tagging**: Emails are tagged automatically using predefined regex patterns.
- **Tag Removal**: Remove tags from emails by clicking a button.
- **Filter Emails**: Filter emails by tags or keywords.
- **Graphical User Interface (GUI)**: Built with Tkinter for easy interaction.

## Requirements

- Python 3.x
- Required libraries:
  - `pywin32` (for interacting with Outlook)
  - `tkinter` (for the GUI)
  - `pandas` (for handling CSV files)
  - `re` (for regular expressions)

You can install the necessary libraries using the following command:
```bash
pip install pywin32 pandas
```

## Configure Your Outlook Email:

In the `fetch_and_tag_emails()` function, you need to specify your Outlook email address.

On line 45, you will see the following line of code:

```python
inbox = outlook.Folders.Item("INPUT_OUTLOOK_EMAIL_HERE").Folders("Inbox")
```
Replace "INPUT_OUTLOOK_EMAIL_HERE" with your actual Outlook email address. For example:

```python
inbox = outlook.Folders.Item("youremail@domain.com").Folders("Inbox")
```
This will allow the program to fetch emails from your Outlook inbox.
