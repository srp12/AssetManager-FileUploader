# Dynamic File Upload - Asset Manager

A premium, animated file upload system designed for healthcare professionals and performance coaches to upload and manage files for their members. Built with the **Cascaid Health Design System** for a professional, modern user experience.

## ✨ Key Features

### 🎨 **Premium Design System**
- **Cascaid Health Branding**: Professional healthcare aesthetic with premium color palette
- **Smooth Animations**: 60+ custom animations and micro-interactions
- **Modern UI Components**: Glass morphism effects, gradient backgrounds, and subtle shadows
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices

### 🚀 **Enhanced User Experience**
- **Animated Page Load**: Staggered entrance animations with professional timing
- **Smart Form Validation**: Real-time feedback with visual error states
- **Loading States**: Progress indicators during file processing
- **Success Celebrations**: Confetti animation and success notifications
- **Ripple Effects**: Material Design-inspired click feedback

### 📁 **Advanced File Management**
- **Drag & Drop**: Enhanced with visual feedback and ripple effects
- **Multi-File Support**: Batch upload with type consistency validation
- **URL Integration**: Direct link addition with format validation
- **File Type Detection**: Automatic categorization with contextual fields
- **Dynamic Table View**: Airtable-style interface for bulk file management

## 🗂️ Supported File Types

### 📄 **PDF Documents**
- **Document Types**: NeuroCatch Report, Quest Bloodwork, Athlete Summary, BodySpec DEXA, Agreements, Other
- **Required Fields**: Document Type, Date of Capture
- **Conditional**: Description (only when "Other" selected)
- **Dynamic Tags**: Context-aware tag suggestions based on document type

### 🖼️ **Images**
- **Image Types**: Training Image, Assessment Image, Progress Photo, Medical Image, Other
- **Required Fields**: Image Type, Date of Capture
- **Smart Tags**: Performance, Training, Assessment, Progress, Development

### 🎥 **Videos**
- **Video Types**: Practice Session, Game Footage, Service Session, Exercise Video, Movement Assessment, Other
- **Required Fields**: Video Type, Date of Capture
- **Contextual Tags**: Dynamic options based on video type selection

### 📊 **Excel Spreadsheets**
- **Document Types**: Data Analysis, Progress Tracking, Report, Other
- **Analytics Tags**: Tracking, Metrics, Performance, Progress

### 📃 **Word Documents**
- **Document Types**: Report, Plan/Program, Notes, Other
- **Professional Tags**: Analysis, Summary, Planning, Documentation

### 🔗 **URL Links**
- **Link Types**: Mammo+ Heart Report, Bone Health Report, Educational Resource, External Assessment, Reference Material, Other
- **Health-Focused**: Specialized options for healthcare resources

## 🎯 **Field Structure**

### **Universal Required Fields**
1. **Asset Type** (contextual label per file type)
2. **Date of Capture**

### **Conditional Fields**
- **Description**: Required only when "Other" is selected
- **Tags**: Multi-select dropdown with contextual options
- **Notes**: Optional for additional information

### **Smart Tag System**
Each asset type provides relevant tag suggestions:
- **NeuroCatch**: Brain Health, Cognitive Assessment, Neurological, Baseline, Follow-up
- **Quest Bloodwork**: Lab Results, Blood Panel, Biomarkers, Health Screening
- **Agreements**: Legal, Consent, Authorization, Privacy, Terms, Records Release
- **Custom Tags**: Users can add their own tags for flexibility

## 🛠️ **Technical Architecture**

### **Design System**
- **CSS Variables**: Consistent spacing (8px base unit), typography scales, and color palette
- **Component Library**: Reusable buttons, forms, cards, and animations
- **Accessibility**: WCAG AA compliant with proper focus management

### **Animation Framework**
- **Entrance Animations**: `fadeInUp`, `slideInLeft`, `fadeInScale`
- **Interaction Feedback**: Ripple effects, hover states, loading spinners
- **Micro-interactions**: Form focus states, tag removal, button feedback
- **Success States**: Confetti celebration, floating success indicators

### **File Structure**
```
Asset Manager - File Upload/
├── index.html              # Main application
├── styles.css              # Cascaid Health Design System
├── README.md              # Documentation
├── PRD_Current_Implementation.txt
└── design.json            # Design system specifications
```

## 🚀 **How to Use**

### **Getting Started**
1. Open `index.html` in a modern web browser
2. Select a member from the dropdown (Serena Williams, LeBron James, Megan Rapinoe)

### **Adding Files**
3. **Drag & Drop**: Files onto the animated upload zone
4. **Browse Files**: Click the upload zone to open file browser
5. **Add URLs**: Enter links in the URL input field

### **Managing Metadata**
6. **Asset Type**: Select appropriate category (auto-updates table header)
7. **Date of Capture**: Required for all files
8. **Tags**: Choose from contextual suggestions or add custom tags
9. **Description**: Required only for "Other" asset types
10. **Notes**: Optional additional information

### **Completing Upload**
11. **Validation**: System highlights missing required fields with animations
12. **Submit**: Click "Upload Files" button (shows loading state)
13. **Success**: Enjoy confetti animation and success notification

## ✅ **Enhanced Features**

### **Visual Feedback**
- ✨ **Loading States**: Buttons show progress during processing
- 🎊 **Success Celebrations**: Confetti animation on completion
- ⚠️ **Smart Errors**: Slide-in notifications with specific guidance
- 🏷️ **Tag Management**: Animated pills with hover effects

### **User Experience**
- 🎯 **Smart Validation**: Real-time field checking with visual feedback
- 📱 **Responsive Design**: Optimized for all screen sizes
- ⌨️ **Keyboard Support**: Full keyboard navigation and shortcuts
- 🎨 **Smooth Transitions**: 300ms standard, 150ms fast, 500ms slow timing

### **Performance**
- 🚀 **Optimized Animations**: Hardware-accelerated CSS transforms
- 📦 **Efficient Loading**: Staggered content appearance
- 🎭 **Reduced Motion**: Respects user accessibility preferences

## 🌟 **Design Highlights**

- **Hero Gradient**: Subtle background with fixed attachment
- **Card Hover Effects**: Lift animation with enhanced shadows
- **Button Interactions**: Gradient backgrounds with ripple feedback
- **Form Focus States**: Subtle lift and blue accent glow
- **Table Animations**: Row hover effects and smooth transitions
- **Tag System**: Contextual multiselect with custom additions

## 💻 **Browser Support**

- **Chrome**: 90+ ✅
- **Firefox**: 88+ ✅
- **Safari**: 14+ ✅
- **Edge**: 90+ ✅

Optimized for modern browsers with graceful degradation for older versions.

## 🏥 **Healthcare-Focused**

Built specifically for healthcare and performance coaching environments:
- **Professional Aesthetic**: Cascaid Health design language
- **Contextual Workflows**: Healthcare-specific document types
- **Compliance Ready**: Structured metadata for record-keeping
- **User-Friendly**: Intuitive interface for busy professionals

---

*Built with modern web technologies and a focus on user experience. No backend required - perfect for prototyping and demonstration purposes.* 