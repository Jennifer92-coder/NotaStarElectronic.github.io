 Automatic Service Invoice Generator (Canvas-Based)

 📌 Overview

This project is a web-based automatic invoice generator designed specifically for service businesses. Users only need to input service details (description and subtotal), and the system will automatically generate a completed invoice image based on a single PNG invoice template using HTML Canvas.

The final invoice can be downloaded as PNG or shared via WhatsApp / Telegram (supported on mobile browsers).



 🎯 Key Features

 🧾 Generate invoices from a single invoice template image (`nota.png`)
 🖊️ Dynamic text rendering using HTML Canvas
 📦 Supports multiple service items
 💰 Automatic total calculation (even if only one item)
 📱 Works on mobile phones and laptops
 ⬇️ Download invoice as PNG
 🔗 Share invoice via WhatsApp / Telegram (mobile-supported browsers)
 📝 Warranty / Guarantee text supports line breaks (Enter) for long sentences



 🛠️ Technologies Used

 HTML5
 CSS3
 JavaScript (Canvas API)

No backend, no database, and no external frameworks required.



 📂 Project Structure

```
project-folder/
│
├── index.html         Main application file
├── nota.png           Invoice template image (blank)
└── README.md          Project documentation
```



 ▶️ How It Works

1. The system loads `nota.png` into an HTML `<canvas>`.
2. User inputs invoice information:

    Invoice number
    Customer name
    Store / service provider
    Date
    Service description
    Quantity (optional)
    Subtotal (direct value, no unit price)
    Warranty / guarantee text
3. JavaScript draws all text at predefined canvas coordinates.
4. The total is calculated automatically from all service subtotals.
5. The completed invoice appears instantly on the canvas.



 🧮 Calculation Logic (Service-Based)

 No unit price is used.
 Each service item directly represents a subtotal.
 Total = sum of all subtotals.
 Total is always displayed, even if only one item exists.



 📝 Warranty / Guarantee Text (Multi-line Support)

Long warranty texts are supported.

 Press Enter to create a new line.
 The text will automatically move down line by line inside the invoice area.
 Prevents text from overflowing horizontally.



 ⬇️ Download Invoice

Click "Download Invoice (PNG)" to save the generated invoice image.

 The downloaded file is taken directly from the canvas, not the blank template.
 File format: PNG



 📤 Share Invoice (WhatsApp / Telegram)

Click "Share to WhatsApp / Telegram":

 Supported on mobile browsers (Chrome, Edge, Safari mobile)
 Uses Web Share API
 If sharing is not supported, users can download the image manually and send it

⚠️ Desktop browsers usually do not support direct image sharing.



 📱 Device Compatibility

| Device        | Status            |
| - | -- |
| Android Phone | ✅ Fully supported |
| iPhone        | ✅ Supported       |
| Laptop / PC   | ⚠️ Download only  |



 ⚠️ Important Notes

 `nota.png` must be in the same folder as `index.html`
 Canvas text positions must match your invoice design
 Works best when opened via:

   Local server
   Hosting (GitHub Pages, Netlify, etc.)



 📌 Use Case Examples

 Service invoices
 Repair receipts
 Freelance service billing
 School / SMK project



 👤 Author:Jennifer

Developed as a learning and project-based web application using pure HTML, CSS, and JavaScript.



 ✅ Status

✔ Stable
✔ Mobile-ready
✔ Offline-capable



If you want:

 PDF export
 Editable invoice template
 Backend saving

Feel free to extend this project 🚀
