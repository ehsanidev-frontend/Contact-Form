# Contact Form Project

A simple, accessible contact form built with **semantic HTML5**.

🔗 **Project Reference:** https://roadmap.sh/projects/contact-form

---

## 📋 Overview

This project is part of the [roadmap.sh](https://roadmap.sh) frontend learning path.  
The goal is to practice building a **semantically correct**, **accessible**, and **well-structured** contact form using only HTML.

---

## 🎯 Objectives

- Use semantic HTML elements (`<header>`, `<main>`, `<footer>`, `<form>`, `<fieldset>`)
- Ensure every form control has a properly associated `<label>`
- Apply correct input types (`text`, `email`, `radio`, `checkbox`, `textarea`, `select`)
- Follow accessibility best practices (label-for/id pairing, fieldset/legend grouping)
- Use native HTML validation (`required`, `minlength`, `type="email"`)

---

## 🧩 Form Fields

| Field | Type | Required | Notes |
|-------|------|----------|-------|
| Full name | `text` | ✅ | `autocomplete="name"` |
| Email | `email` | ✅ | `autocomplete="email"` |
| Subject | `select` | ✅ | Options: Debugging, Collaboration |
| Message | `textarea` | ✅ | `minlength="10"` |
| Referral source | `radio` | ✅ | Search / Friend / Social media |
| Newsletter | `checkbox` | ❌ | Optional opt-in |
| Submit | `button` | — | Sends the form |

---

## ✅ Accessibility Checklist

- [x] Every input has a `<label>` with matching `for` / `id`
- [x] Radio buttons are grouped inside a `<fieldset>` with a `<legend>`
- [x] Each radio and checkbox is wrapped in its own `<label>`
- [x] Form controls use appropriate `type` attributes
- [x] Native validation via `required` and `minlength`
- [x] Autocomplete attributes for name and email

---

## 🐛 Known Issues (Original Version)

The initial version of the form had the following problems:

1. `for` attributes did not match input `id`s (name, email, subject, message)
2. `select` and `textarea` were missing `name` attributes → data not submitted
3. Radio buttons and checkbox were not associated with labels
4. Radio buttons were missing `value` attributes
5. `action="..."` was a placeholder
6. No `required` attributes on mandatory fields
7. No `autocomplete` attributes

All of the above have been fixed in the revised version.

---

## 🚀 How to Use

1. Clone or download the repository.
2. Open `contact.html` in any modern browser.
3. Fill in the form and submit (backend endpoint to be added later).

---

## 🛠️ Tech Stack

- HTML5 only (no CSS/JS yet — styling and validation to be added in future iterations)

---

## 🔮 Future Improvements

- [ ] Add CSS styling (responsive, mobile-first)
- [ ] Add client-side JS validation
- [ ] Connect to a real backend endpoint
- [ ] Add ARIA attributes where needed
- [ ] Add tests with a tool like Playwright or Cypress
- [ ] Improve error messaging UI

---

## 📄 License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).