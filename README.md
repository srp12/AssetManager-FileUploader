# Dynamic File Upload Prototype

A high-fidelity, interactive HTML prototype for a dynamic file upload system designed for performance coaches and clinicians to upload files for their members.

## Features

### Core Functionality
- **Member Selection**: Choose from a dropdown of mock members (Serena Williams, LeBron James, Megan Rapinoe)
- **File Upload**: Drag & drop or click to browse for files (supports multiple file selection)
- **URL Links**: Add files via URL input
- **Dynamic Forms**: Conditional fields that appear based on file type
- **Multi-File Type Validation**: Prevents mixing different file types in the same upload batch
- **Form Validation**: Required field validation with visual feedback
- **File Type Indicator**: Shows current batch type when files are added
- **Responsive Design**: Works on desktop and mobile devices

### Supported File Types
- 📄 **PDF** (.pdf) - Requires document type selection before showing additional fields
- 🖼️ **Images** (.jpg, .png, .gif) - Standard metadata fields
- 🎥 **Videos** (.mp4, .mov) - Standard metadata fields  
- 📊 **Excel** (.xls, .xlsx) - Standard metadata fields
- 📃 **Word** (.doc, .docx) - Standard metadata fields
- 🔗 **URLs** - Direct link addition with metadata

### Conditional Logic

#### PDF Files
1. First shows "Document Type" dropdown with options:
   - NeuroCatch Report
   - Quest Bloodwork
   - Athlete Summary
   - BodySpec DEXA
   - Other
2. After selection, reveals required fields: Description, Tags, Goals, Date of Capture
3. Optional field: Notes

#### Video Files  
1. First shows "Video Type" dropdown with options:
   - Practice Session
   - Game Footage
   - Service Session
   - Exercise Video
   - Other
2. After selection, reveals:
   - Required fields: Description, Tags, Date of Capture
   - Contextual multi-select tags based on video type:
     - **Practice Session**: Warmup, Drills, Scrimmage, Cool Down, Team Practice, Individual Practice
     - **Game Footage**: Highlights, Full Game, Key Plays, Performance Analysis, Team Strategy, Individual Performance
     - **Service Session**: Assessment, Treatment, Consultation, Follow-up, Education, Therapy
     - **Exercise Video**: Strength Training, Cardio, Flexibility, Balance, Rehabilitation, Sport Specific
     - **Other**: Analysis, Review, Documentation, Reference, Educational, Promotional
3. Optional fields: Goals, Notes

#### Other File Types
Show immediate required fields:
- Description (text area)
- Tags (text input)
- Date of Capture (date picker)

Optional fields vary by type (Goals, Notes)

## How to Use

1. **Open the File**: Open `index.html` in any modern web browser
2. **Select Member**: Choose a member from the dropdown (required)
3. **Add Files**: 
   - Drag and drop files onto the upload zone, OR
   - Click the upload zone to browse files, OR
   - Enter a URL in the URL input field and click "Add URL"
4. **Fill Metadata**: Complete the required fields that appear for each file
5. **Validate**: The system will highlight missing required fields
6. **Submit**: Click "Upload Files" to complete the process
7. **Success**: See confirmation message and cleared form

## Technical Details

- **Stack**: Plain HTML, Tailwind CSS (via CDN), Vanilla JavaScript
- **File Detection**: Uses file extensions and MIME types
- **Validation**: Client-side validation with visual feedback
- **No Backend**: This is a prototype - no actual file uploads occur
- **Responsive**: Built with Tailwind CSS for mobile/desktop compatibility

## File Structure
```
Asset Manager - File Upload/
├── index.html          # Main application file
└── README.md          # This documentation
```

## Requirements Met
✅ Member selection dropdown  
✅ Drag & drop file upload  
✅ Alternative file browser  
✅ URL input functionality  
✅ Dynamic file cards  
✅ Conditional field logic  
✅ PDF document type workflow  
✅ **Video type conditional workflow**  
✅ **Contextual multi-select video tags**  
✅ **Multi-file upload support**  
✅ **File type mixing validation**  
✅ Form validation  
✅ Error highlighting  
✅ Success messaging  
✅ File removal capability  
✅ **File type batch indicator**  
✅ Responsive design  
✅ Professional styling  

## Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

The prototype uses modern JavaScript features but maintains broad browser compatibility. 