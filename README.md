# OpenDocket — Free Legal Forms for Everyone

![Open Docket](https://img.shields.io/badge/Open%20Docket-Free%20%26%20Open%20Source-0B1F3A?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-C9A84C?style=for-the-badge)
![No Signup](https://img.shields.io/badge/No%20Signup-Required-2D6A4F?style=for-the-badge)

> *Not everyone can afford a lawyer to find the right form. Not everyone knows what forms even exist. Open Docket was built for them.*

---

## What is Open Docket?

Open Docket is a completely free, open source legal form finder that speaks plain English.

Search hundreds of federal and state government forms by your situation — not by form number. Every form comes with:

- **Plain language explanation** of what the form actually does
- **Who needs it** — described in everyday terms, not legal jargon
- **Step-by-step instructions** for completing and submitting it
- **What happens next** — so you know what to expect after you file
- **Direct link** to the official government source

No subscriptions. No signups. No lawyer required. Just open the page and find what you need.

---

## Who This Is For

Open Docket was built for people who have been left behind by a legal system that assumes everyone can afford professional help:

- 👩‍👧 Single parents navigating custody or child support
- 👴 Elderly individuals dealing with Medicare, Social Security, or benefits
- 🌎 Immigrants trying to understand USCIS forms
- 🏘️ Renters facing eviction or fighting for their security deposit
- ⚖️ Anyone who got blindsided by a situation they've never faced before
- 💸 People who simply cannot afford $300/hour for an attorney

---

## Categories Covered

| Category | Examples |
|---|---|
| 🏠 **Housing** | Eviction response, security deposit demand, Section 8 approval |
| 💳 **Bankruptcy** | Chapter 7, Chapter 13, means test |
| 💼 **Employment** | Unemployment insurance, wage theft, workplace discrimination |
| 👨‍👩‍👧 **Family** | Child custody, child support enforcement, name change |
| 🌎 **Immigration** | Green card, DACA renewal, green card replacement |
| 🎖️ **Veterans** | VA disability compensation, GI Bill education benefits |
| 🏥 **Healthcare** | Medicare Part B enrollment, Social Security disability (SSDI) |
| ⚖️ **Small Claims** | How to sue for money owed without a lawyer |

---

## How to Use It

1. **Open `opendocket.html`** in any web browser — no installation needed
2. **Search** by describing your situation in plain English
3. **Filter** by category or state
4. **Click any form** to see the full plain-language explanation
5. **Click "Get Official Form"** to go directly to the government source

That's it. No account. No email. No cost.

---

## Running Locally

No setup required. Just download and open:

```bash
git clone https://github.com/YOUR-USERNAME/open-docket.git
cd open-docket
open opendocket.html
```

Or simply download the file and double-click it.

---

## Contributing

Open Docket is a community project. The more forms we add, the more people we help.

### How to add a form

Each form in the database follows this structure:

```javascript
{
  id: 21,                          // Next available ID
  category: "housing",             // Category slug
  catLabel: "Housing",             // Display label
  num: "FORM-NUMBER",              // Official form number
  title: "Official Form Name",     // Full form title
  plain: "One sentence plain English summary.",
  who: "Describe who needs this form in plain language.",
  what: "Full plain English explanation of what this form does and why it matters.",
  steps: [
    "First thing the person needs to do",
    "Second step",
    "Third step"
  ],
  after: "What happens after the form is submitted.",
  link: "https://official-government-source.gov",
  state: "federal",                // "federal", "all", or state code e.g. "TN"
  tags: ["keyword1", "keyword2"]   // Search keywords
}
```

### To contribute:
1. Fork this repository
2. Add your form to the `FORMS` array in `opendocket.html`
3. Submit a pull request with a brief description of the form you added
4. That's it — no coding experience required beyond copy/paste

### What makes a good contribution:
- Forms that real people commonly need but struggle to find
- Plain language that a 10th grader can understand
- Accurate links to official `.gov` sources only
- Correct form numbers and up-to-date information

---

## Roadmap

Things we want to build next:

- [ ] All 50 states with state-specific forms
- [ ] Spanish language support
- [ ] Printable form checklists
- [ ] "I don't know what I need" guided questionnaire
- [ ] Legal aid clinic finder by zip code
- [ ] More bankruptcy forms (Schedule A through J)
- [ ] Small business forms
- [ ] Tenant rights by state
- [ ] Form update notifications when government forms change

---

## License

MIT License — free to use, modify, and distribute. See `LICENSE` for details.

---

## Disclaimer

Open Docket provides general information about government forms only. It does not provide legal advice. The information on this site is not a substitute for advice from a licensed attorney. For complex legal matters, please consult a qualified legal professional or contact your local legal aid organization.

**Find free legal help near you:** [lawhelp.org](https://www.lawhelp.org)

---

## Support the Project

Open Docket will always be free. If you find it helpful:

- ⭐ Star this repository
- 🔁 Share it with someone who needs it
- 🛠️ Contribute a form
- 📣 Tell your local legal aid organization about it

---

*Built with the belief that understanding your legal rights shouldn't depend on how much money you have.*
