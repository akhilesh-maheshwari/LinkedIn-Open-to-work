# 🚀 LinkedIn Profile Open to Work Status

Accurately detect whether a LinkedIn profile is marked as Open to Work. Submit a LinkedIn person profile URL and receive a simple true or false result.

This Actor is useful for recruitment, candidate sourcing, talent intelligence, profile enrichment, and automated hiring workflows.

No LinkedIn login or cookies required.

---

## ✨ Features

- **Detect Open to Work status:** Check whether a LinkedIn profile is currently marked as Open to Work
- **Simple boolean result:** Receive true or false for easy processing
- **No cookies required:** Run without LinkedIn login cookies or an active session
- **Easy integration:** Use the output in CRMs, spreadsheets, ATS platforms, and automation tools
- **Automation-ready:** Connect through the Apify API, webhooks, n8n, Make, Zapier, or custom scripts

---

## 📥 Input

Provide the public LinkedIn profile URL you want to check.

| Field | Required | Description |
|---|---|---|
| `linkedin_url` | Yes | Public LinkedIn person profile URL |

### Input Example

```json
{
  "linkedin_url": "https://www.linkedin.com/in/ajjames"
}
```

---

## 📤 Output

The Actor returns the profile's Open to Work status inside the data object.

| Field | Description |
|---|---|
| `data.open_to_work` | `true` when the profile is marked as Open to Work; otherwise `false` |
| `message` | Status message returned by the Actor |

### Output Example

```json
{
  "data": {
    "open_to_work": false
  },
  "message": "ok"
}
```

---

## 🔎 Understanding the Result

- `"open_to_work": true` means the LinkedIn profile was detected as Open to Work.
- `"open_to_work": false` means the profile was not detected as Open to Work.

The result reflects the profile information available at the time of the request.

---

## 📁 How to Use

1. Create or sign in to your Apify account.
2. Open the LinkedIn Profile Open to Work Status Actor.
3. Paste a public LinkedIn person profile URL into `linkedin_url`.
4. Run the Actor.
5. View the boolean result in the output dataset.
6. Export the result or connect it to your workflow through the Apify API.

---

## 🧠 Common Use Cases

- **Candidate sourcing:** Identify profiles that may be open to new opportunities
- **Recruitment prioritization:** Prioritize candidates who are actively exploring roles
- **Talent database enrichment:** Add Open to Work status to candidate records
- **ATS and CRM workflows:** Update recruiting systems using a simple boolean field
- **Automated screening:** Add availability signals to recruitment workflows
- **Market research:** Analyze Open to Work signals across professional profiles

---

## ⚠️ Data Availability

The Actor checks the Open to Work signal available for the submitted LinkedIn profile. Profile visibility and LinkedIn settings may affect the returned result. A `false` value means the Open to Work status was not detected at the time of processing.

Use the returned data responsibly and follow applicable privacy and data-protection requirements.
