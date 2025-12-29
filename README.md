# PDF to Word Converter

A Robotic Process Automation (RPA) project built with UiPath that automatically converts PDF files to Microsoft Word documents.

## Description

This UiPath automation project reads PDF files from the `InputPDFs` folder and converts them to Word documents, saving the output in the `OutputDocs` folder. The automation handles the conversion process efficiently, making it easy to batch convert multiple PDF files.

## Features

- Automated PDF to Word conversion
- Batch processing of multiple PDF files
- Organized input and output folder structure
- Error handling and logging capabilities

## Prerequisites

- **UiPath Studio** (version 2023.10 or later recommended)
- **Microsoft Word** installed on the system
- **Windows Operating System**

## Project Structure

```
PDFtoWord/
├── Main.xaml                    # Main workflow entry point
├── ConvertPDFToWord.xaml        # PDF conversion workflow
├── Sequence.xaml               # Additional workflow sequences
├── trial.xaml                  # Test/trial workflow
├── project.json               # UiPath project configuration
├── InputPDFs/                 # Folder for input PDF files
├── OutputDocs/                # Folder for output Word documents
└── README.md                  # This file
```

## Dependencies

The project uses the following UiPath packages:

- UiPath.PDF.Activities (v3.22.1) - For PDF manipulation
- UiPath.Word.Activities (v2.0.1) - For Word document creation
- UiPath.System.Activities (v25.4.2) - Core system activities
- UiPath.UIAutomation.Activities (v25.10.3) - UI automation capabilities
- UiPath.IntegrationService.Activities (v1.15.0) - Integration services

## Setup Instructions

1. **Clone or Download** the project files to your local machine
2. **Open UiPath Studio**
3. **Open Project**: File → Open → Project/Solution → Navigate to the project folder and select `project.json`
4. **Restore Dependencies**: UiPath Studio will automatically restore the required packages
5. **Verify Folders**: Ensure the `InputPDFs` and `OutputDocs` folders exist in the project directory

## How to Run

1. **Place PDF files** in the `InputPDFs` folder
2. **Open Main.xaml** in UiPath Studio
3. **Run the project** by clicking the "Run" button or pressing F5
4. **Check Output**: Converted Word documents will be saved in the `OutputDocs` folder

## Configuration

The automation can be configured by modifying the workflow files:

- **Main.xaml**: Controls the overall process flow
- **ConvertPDFToWord.xaml**: Contains the core conversion logic
- **Input/Output Paths**: Modify folder paths in the workflows as needed

## Troubleshooting

- Ensure Microsoft Word is properly installed and accessible
- Check that input PDF files are not password-protected
- Verify that the output folder has write permissions
- Review UiPath Studio logs for detailed error information

## Notes

- This project requires user interaction for certain operations (as configured in project.json)
- The automation is designed for attended execution
- Large PDF files may take longer to convert depending on system resources
