# Asha Kiran Foundation Website

A responsive, one-page website for **Asha Kiran Foundation**, a fictional NGO that runs learning centres, community kitchens and health camps. The site includes a donation form and a volunteer sign-up form, both with JavaScript validation.

Built with plain **HTML5, CSS3 and JavaScript**. There are no frameworks and no build steps.

---

## Features

- Sticky navigation bar with anchor links (About, Programs, Donate, Volunteer)
- Hero banner with a "Donate Now" call to action
- "Who We Are" section describing the foundation
- Program cards: Learning Centres, Community Kitchen, Health Camps
- **Donation form**
  - Preset amount buttons (Rs. 500, Rs. 1500, Rs. 5000)
  - Validation for name, email and amount
  - Thank-you message on success
- **Volunteer form**
  - Validation for name, a 10-digit phone number and an area of interest
  - Confirmation message on success
- Fully responsive layout (flexbox and a media query for screens up to 600px)

---

## Tech Stack

| Technology | Used for |
|---|---|
| HTML5 | Page structure and forms |
| CSS3 | Styling, flexbox layout, hover effects, responsive design |
| JavaScript (inline) | Form validation, DOM updates, preset amount buttons |

---

## Project Structure

```
.
├── index.html      # Page structure and inline JavaScript
├── style.css       # All styling and responsive rules
├── images.jpg      # Foundation logo (not yet used on the page)
└── settings.json   # VS Code Live Preview setting (opens /index.html)
```

---

## Getting Started

### Option 1: Open directly
1. Clone or download this repository.
2. Open `index.html` in any modern browser.

### Option 2: VS Code Live Preview
1. Open the folder in VS Code.
2. Install the **Live Preview** extension.
3. Right-click `index.html` and choose **Show Preview**.

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
```

---

## How the Forms Work

**Donation form**
- Name must not be empty.
- Email must not be empty and must contain `@` and `.`.
- Amount must be greater than 0.
- On success, a thank-you message is shown and the form resets.

**Volunteer form**
- Name must not be empty.
- Phone must be exactly 10 digits (checked with the regular expression `/^\d+$/`).
- An area of help must be selected.
- On success, a confirmation message is shown and the form resets.

> **Note:** This is a front-end demo. No data is sent to a server, stored, or processed, and no real payment takes place.

---

## Possible Improvements

- Add the foundation logo (`images.jpg`) to the header or hero section
- Connect the forms to a backend and database
- Integrate a payment gateway (for example Razorpay) for real donations
- Use stronger email validation and add server-side validation
- Send confirmation emails to donors and volunteers
- Improve accessibility (ARIA labels, keyboard focus styles)

---

## Author

**<Your Name>**
GitHub: [@<your-username>](https://github.com/<your-username>)

---

## License

This project was created for educational purposes. You are free to use and modify it for learning.
