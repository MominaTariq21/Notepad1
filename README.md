

This Notepad Web App is an online text editor that provides functionalities for writing, editing, and saving plain text documents. It includes features like:

Rich text editing powered by TinyMCE.

File upload for .txt files.

Save functionality to download edited files.

Spellchecking, word counting, and autosave.

Project Structure

HTML Structure

<div class="app">: Main container for the application.

Title Bar: Displays the app title as a link.

TinyMCE Editor: A <textarea> element enhanced by TinyMCE for rich text editing.

File Input: A hidden <input> element for uploading .txt files.

CSS Styling

Styles are defined in an external stylesheet (style.css) and some inline styles:

Responsive Design: Media queries are used to adjust ad banner sizes based on screen width.

Editor Layout: Styles for #editor ensure full-width and height usage.

Visual Elements: Gradients, box shadows, and rounded corners provide a polished design.

JavaScript

TinyMCE Initialization:

Configured with plugins like autosave, wordcount, and spellchecker.

Toolbar includes options for formatting, alignment, and basic text editing commands.

File Handling:

Uses FileReader to load .txt files into the editor.

Blob objects and anchor tags enable saving text as .txt files.

Event Listeners:

Listens for file uploads and key shortcuts (e.g., Ctrl+S to save files).

Features

Text Editing

Rich text editing via TinyMCE.

Autosave functionality ensures your notes are backed up periodically.

Browser spellchecking and word count support.

File Handling

File Upload: Users can upload .txt files to edit.

Files are read and loaded into the editor using JavaScript.

Save File: Edited text can be saved locally as a .txt file.

Uses Blob API and dynamic anchor tags for file download.

Customization

The editor is configured to enforce plaintext input (no HTML formatting).

Keyboard shortcuts like Ctrl+S for saving are integrated for ease of use.

Usage Instructions

Setup

Open the index.html file in your browser.

The editor will load, ready for text input.

Editing Text

Begin typing directly in the editor.

Use the toolbar for basic text manipulation.

File Upload

Click on the "Open..." option or use the file input.

Select a .txt file from your computer.

The contents will be loaded into the editor for editing.

Save File

Click on "Save" or press Ctrl+S.

A download prompt will appear with the file name.

File Details

HTML File

Contains the layout and structure of the Notepad app.

Uses external CSS and JavaScript files for styling and functionality.

CSS Files

/css/style.css: General styles for the application.

/css/notepad3.css: Additional editor-specific styles.

JavaScript

cfg.js: Contains TinyMCE configuration and file handling logic.

Dependencies

TinyMCE: Rich text editor library.

jQuery: Used for DOM manipulation and event handling.

Blob API: Enables file saving functionality.

