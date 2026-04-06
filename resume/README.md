# ATS-Optimized Resume Template

A single-page HTML resume template with exact A4 sizing and PDF export capability. Designed to be ATS (Applicant Tracking System) friendly while maintaining a professional appearance.

## Features

✅ **ATS-Compatible**: All text is selectable and parsable by resume screening systems  
✅ **Exact A4 Sizing**: 210mm × 297mm with precise CSS control  
✅ **PDF Export**: One-click export via browser's native print-to-PDF  
✅ **No Dependencies**: Pure HTML/CSS, works offline  
✅ **Print-Optimized**: Separate styling for screen and print  
✅ **Page Break Control**: Prevents awkward section breaks  
✅ **Professional Design**: Clean, modern layout using ATS-friendly fonts  

## Quick Start

1. Open `index.html` in your web browser
2. Edit the content with your information
3. Click "Download as PDF" button
4. In the print dialog, select "Save as PDF"
5. Your resume is ready to submit!

## How to Edit

Simply open `index.html` in any text editor and replace the placeholder content:

### Sections to Update:

- **Header**: Your name and contact information
- **Professional Summary**: Brief overview of your experience
- **Work Experience**: Job titles, companies, dates, and achievements
- **Education**: Degrees, schools, and relevant coursework
- **Skills**: Technical skills, soft skills, tools, and languages
- **Certifications**: Professional certifications (optional)
- **Projects**: Notable projects (optional)

### Tips for ATS Optimization:

1. **Use standard section headings**: "Work Experience", "Education", "Skills"
2. **Include keywords** from the job description naturally
3. **Use bullet points** for achievements (start with action verbs)
4. **Quantify results** when possible (e.g., "Increased sales by 25%")
5. **Avoid tables** for critical information
6. **Use standard fonts**: Calibri, Arial, Times New Roman
7. **Keep formatting simple**: Bold and italics only
8. **Don't put important info in headers/footers**

## PDF Export Instructions

### Method 1: Using the Button (Recommended)
1. Click the "📄 Download as PDF" button
2. In the print dialog:
   - **Destination**: Save as PDF
   - **Paper size**: A4
   - **Margins**: Default
   - **Scale**: 100%
3. Click "Save"

### Method 2: Keyboard Shortcut
- **Windows/Linux**: Press `Ctrl + P`
- **Mac**: Press `Cmd + P`
- Follow the same print dialog steps above

## A4 Size Specifications

The resume is configured for exact A4 paper dimensions:
- **Width**: 210mm (8.27 inches)
- **Height**: 297mm (11.69 inches)
- **Content Padding**: 20mm on all sides
- **Print Margins**: 15mm (configurable in `@page` CSS)

## Customization

### Changing Colors

Find the color codes in the `<style>` section:
```css
/* Primary color (section borders, button) */
#2563eb → Change to your preferred color

/* Text colors */
#1a1a1a → Headings
#333 → Body text
#666 → Dates
```

### Adjusting Spacing

Modify the spacing values in the CSS:
```css
.section {
    margin-bottom: 16pt; /* Space between sections */
}

.job {
    margin-bottom: 12pt; /* Space between jobs */
}
```

### Adding/Removing Sections

Simply copy/paste section blocks:
```html
<div class="section">
    <h2>Section Title</h2>
    <!-- Your content here -->
</div>
```

## Multi-Page Resumes

If your resume extends beyond one page:

1. The template automatically handles page breaks
2. Sections won't break awkwardly (controlled by `page-break-inside: avoid`)
3. Each page will be exactly A4-sized
4. To force a page break before a section, add:
   ```css
   .specific-section {
       page-break-before: always;
   }
   ```

## Browser Compatibility

Works in all modern browsers:
- ✅ Chrome/Edge (Recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Opera

## Troubleshooting

### PDF doesn't match screen preview
- Ensure print scale is set to 100%
- Check that "Print backgrounds" is enabled
- Verify paper size is set to A4

### Text not selectable in PDF
- Make sure you're using "Save as PDF" not "Print to PDF" with a physical printer selected
- This template uses native browser printing, so text will always be selectable

### Content cut off
- Reduce content padding in `.resume-container`
- Adjust `@page` margins
- Consider using a smaller font size

### ATS not parsing correctly
- Ensure you're using standard section headings
- Avoid complex layouts or tables
- Test your PDF with an ATS parser tool online

## File Structure

```
resume/
├── index.html          # Main resume file (this is all you need!)
└── README.md          # This documentation
```

## License

Free to use and modify for personal and commercial purposes.

## Support

For issues or questions, refer to the CSS comments in `index.html` for detailed explanations of each section.

---

**Pro Tip**: Keep a master copy of your resume and create customized versions for different job applications by adjusting keywords and emphasizing relevant experience.
