# AI Page Designer Prompt

Use this prompt with AI page generators/designers (e.g., v0.dev, Galileo AI, Uizard, etc.) to create the HTML resume/portfolio page.

---

## Prompt for AI Designer

```
Create a modern, professional single-page HTML resume and portfolio website for a software developer with the following requirements:

LAYOUT & STRUCTURE:
- Single HTML file with embedded CSS and minimal JavaScript
- Fully responsive design (mobile-first approach)
- Smooth scrolling between sections
- Fixed navigation header that becomes sticky on scroll
- Footer with social links and contact information

SECTIONS (in order):
1. Hero Section
   - Full-screen or large hero with name, professional title, and tagline
   - Subtle animated background or gradient
   - Call-to-action buttons: "View Portfolio" and "Talk to HR Agent"
   - Professional headshot (placeholder for now)

2. About Me
   - Brief professional summary (2-3 paragraphs)
   - Key highlights in a visually appealing grid or card layout
   - Download resume button

3. Technical Skills
   - Categorized skill sections (Languages, Frameworks, Tools, etc.)
   - Visual representation (skill bars, tags, or icon grid)
   - Modern, clean presentation

4. Work Experience
   - Timeline or card-based layout
   - Company name, role, duration, and key achievements
   - Expandable/collapsible details for each role

5. Projects Portfolio
   - Grid layout (2-3 columns on desktop, 1 on mobile)
   - Project cards with:
     - Project thumbnail/screenshot
     - Title and brief description
     - Technologies used (as tags)
     - Links to demo/GitHub
   - Hover effects for interactivity

6. Education & Certifications
   - Clean list or card layout
   - Institution, degree, year
   - Relevant certifications

7. Contact Section
   - Contact form (name, email, message)
   - Social media links
   - Email and location info

8. Chatbot Widget
   - Fixed position chat button (bottom-right corner)
   - Floating action button style
   - Opens chat interface when clicked
   - Chat interface should include:
     - Header with title "HR Agent"
     - Message area with scrollable chat history
     - Input field and send button
     - Close button
     - Typing indicator placeholder
   - Modern chat UI design (similar to Intercom, Drift, or modern messaging apps)

DESIGN STYLE:
- Modern, minimalist aesthetic
- Professional but approachable
- Color scheme: Use a sophisticated palette (e.g., dark navy/blue primary, accent color for CTAs, neutral grays, white backgrounds)
- Typography: Modern sans-serif fonts (e.g., Inter, Poppins, or similar)
- Generous white space
- Subtle shadows and depth
- Smooth transitions and hover effects
- Glass-morphism or subtle gradients for visual interest

TECHNICAL REQUIREMENTS:
- Pure HTML/CSS/JavaScript (no frameworks)
- Mobile-responsive (breakpoints for mobile, tablet, desktop)
- Semantic HTML5
- Accessible (ARIA labels, proper heading hierarchy)
- Fast loading (optimized CSS, minimal JavaScript)
- Cross-browser compatible
- SEO-friendly meta tags

CHATBOT WIDGET SPECIFICATIONS:
- Chat button: 60px circle, fixed bottom-right (20px from edges)
- Chat window: 400px wide × 600px tall on desktop, full-screen on mobile
- Smooth slide-in animation when opened
- Modern message bubbles (user messages right-aligned, agent left-aligned)
- Timestamp display
- Professional color scheme matching the main site
- Input field with auto-resize
- Send button or Enter key to submit

INTERACTIVE ELEMENTS:
- Smooth scroll to sections when clicking navigation
- Fade-in animations on scroll
- Hover effects on cards and buttons
- Form validation for contact form
- Responsive navigation (hamburger menu on mobile)

PLACEHOLDER CONTENT:
- Name: Khanin Chomphusri
- Domain: khanin.ch
- Use Lorem Ipsum or generic placeholder text for other content sections
- Use placeholder images (e.g., https://via.placeholder.com)
- Include comments in HTML indicating where to replace with actual content

OUTPUT:
- Single index.html file
- Well-commented code
- Organized CSS (use CSS custom properties for colors/spacing)
- Clean, readable code structure
- Include instructions for customization

INSPIRATION:
- Modern developer portfolios
- Clean SaaS landing pages
- Professional resume websites
- Contemporary chat interfaces (Intercom, Drift style)

Make it production-ready, visually stunning, and highly professional while maintaining simplicity and fast performance.
```

---

## Additional Customization Notes

After generating the initial design, you may want to request:

1. **Color Scheme Variations**
   - "Make it darker with a dark mode aesthetic"
   - "Use a specific brand color: #[HEX_CODE]"
   - "Create a light/airy version with pastel colors"

2. **Layout Adjustments**
   - "Make the hero section more compact"
   - "Add a side navigation for larger screens"
   - "Reorganize sections in a different order"

3. **Animation Enhancements**
   - "Add more scroll animations"
   - "Include particle effects in the hero section"
   - "Add typing animation for the tagline"

4. **Chatbot Customization**
   - "Make the chat widget more prominent"
   - "Add a welcome message that auto-appears"
   - "Include suggested questions as quick-reply buttons"

---

## Testing Checklist

After receiving the generated page, test:
- [ ] Responsive design on mobile, tablet, desktop
- [ ] All navigation links work
- [ ] Chatbot opens/closes smoothly
- [ ] Forms have proper validation
- [ ] All animations are smooth (60fps)
- [ ] Page loads quickly
- [ ] Accessible via keyboard navigation
- [ ] Works in Chrome, Firefox, Safari, Edge
- [ ] SEO meta tags are present
- [ ] No console errors

---

## Integration Points

Remember that the generated HTML will need:
1. **Content replacement** - Fill in your actual resume/portfolio content
2. **Chatbot JavaScript** - Connect to the Render.com backend API
3. **Images** - Replace placeholders with actual photos/screenshots
4. **Analytics** - Add Google Analytics or similar (optional)
5. **SEO** - Update meta tags with actual information
