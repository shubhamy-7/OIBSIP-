# Web Dev L1 — Task 3: Temperature Converter Website

**Track:** Web Development & Designing — Level 1
**Task:** Temperature Converter Website
**Author:** Shubham Yadav

## Objective

An interactive web tool that converts temperature values between Celsius, Fahrenheit, and Kelvin, with real-time input validation and a thermometer visual that reflects the converted result.

## Tech Stack

- HTML5
- CSS3
- JavaScript (Vanilla)
- Google Fonts: Space Grotesk (display), Inter (body), JetBrains Mono (numeric readouts)

## Features

- Numeric input field for the temperature value, with validation that rejects non-numeric input and shows a clear inline error message
- Input unit selector (°C / °F / K toggle buttons) letting the user choose the unit they're entering
- Auto-conversion display: all three output units (Celsius, Fahrenheit, Kelvin) are shown simultaneously after conversion — no need to pick an output unit separately
- Convert button that triggers the calculation on click (Enter key also works)
- Result display area with correctly labelled, precisely formatted values
- Edge case handling: any input equivalent to below absolute zero (−273.15°C / −459.67°F / 0K) shows a friendly explanatory message instead of a raw calculation error
- A thermometer visual that fills and shifts colour (blue → red) based on the converted Celsius value, giving a second, at-a-glance read of the result
- Clean, centred UI layout with clear labels, fully responsive (thermometer switches to a horizontal layout on mobile)

## Conversion Formulas Used

- Celsius → Fahrenheit: `F = C × (9/5) + 32`
- Fahrenheit → Celsius: `C = (F − 32) × (5/9)`
- Celsius → Kelvin: `K = C + 273.15`
- Kelvin → Celsius: `C = K − 273.15`

## File Structure

```
OIBSIP/WebDev-L1-TemperatureConverter/
├── index.html
└── README.md
```

## How to View

Open `index.html` directly in any modern browser — no build step or server required.

## Notes

Input validation uses a regular expression (`^-?\d*\.?\d+$`) to accept optional negative signs and decimals while rejecting letters, symbols, or empty submissions.

---
*Submitted as part of the Oasis Infobyte Summer Internship Program (OIBSIP) — Web Development & Designing track.*
