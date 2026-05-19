# GLIO AI-Automation — Google Ads pack (copy-paste ready)

Landing page: **https://omarkhalawi21.github.io/glio-ai-automation/**
Send every ad to that URL. Goal conversion: **WhatsApp click**.

> Char limits Google enforces: **Headlines ≤ 30**, **Descriptions ≤ 90**.
> All copy below is within limits.

---

## 1. Campaign settings

- **Type:** Search (uncheck "Display Network" and "Search partners" to start)
- **Goal:** Leads
- **Locations:** Saudi Arabia, UAE, Kuwait, Qatar, Bahrain, Oman (add UK/US only if you serve them). Target *"people in your locations"*, not "interested in".
- **Languages:** Arabic + English
- **Bidding:** start **Maximize clicks** with a max-CPC cap (~SAR 6–10) for the first ~2 weeks of data, then switch to **Maximize conversions** once the WhatsApp conversion has ~15+ records.
- **Budget:** start **SAR 60–90/day**. One campaign, the 4 ad groups below.
- **Ad rotation:** Optimize. **Ad schedule:** all week (B2B leans Sun–Thu daytime KSA; refine later from data).

## 2. Conversion tracking (do this before launch — ads are blind without it)

The page already fires a `generate_lead` event on WhatsApp/email/call clicks.
1. Create a **GA4** property → copy its ID (`G-XXXXXXXXXX`).
2. In `index.html`, set `window.GLIO_GA = "G-XXXXXXXXXX";` → commit/push.
3. In GA4, mark `generate_lead` as a **Key event**.
4. Link GA4 to Google Ads → **import** `generate_lead` as a conversion.
   (Or use a Google Ads click conversion on the same event.)

---

## 3. Ad groups

### AG1 — AI automation (core intent)
**Keywords** (phrase + exact):
```
"ai automation for business"   [ai automation for business]
"business process automation"  "automate my business"
"ai automation company"        "ai automation services"
"hire ai automation"           "ai automation consultant"
```
**Headlines:**
```
AI Automation, Done For You
Stop Doing Manual Work
AI Automation for Business
Automate the Repetitive Work
Free Automation Audit
Done-For-You AI Automation
We Build It & We Run It
Get Your Hours Back
Bilingual KSA AI Team
Automation That Pays Off
From Audit to Live in Weeks
Talk to Us on WhatsApp
AI That Runs Your Busywork
Cut Cost, Not Headcount
Built Around Your Workflow
```
**Descriptions:**
```
We map, build & run AI automation for your business. Free audit on WhatsApp.
Stop paying people for work a machine should do. Done-for-you. Book a free audit.
Customer support, data entry, reporting, follow-ups — automated. KSA-based team.
Bilingual team in Al Khobar. ROI-priced. Live in 2–4 weeks. Message us today.
```

### AG2 — Customer-support / chatbot automation
**Keywords:** `"automate customer support"  "ai customer service"  "whatsapp chatbot for business"  "ai chatbot company"  "customer support automation"`
**Headlines (swap 4–5 into the AG1 set):**
```
Automate Customer Support
24/7 AI Customer Replies
AI Chatbot, Arabic & English
Answer Customers Instantly
Cut Support Workload
WhatsApp & Web AI Support
```
**Description:**
```
An AI assistant that answers customers 24/7 in Arabic & English. Free audit.
```

### AG3 — Workflow / data-entry / reporting
**Keywords:** `"automate data entry"  "workflow automation agency"  "automate reporting"  "rpa for small business"  "automate back office"`
**Headlines:**
```
Automate Data Entry
No More Copy-Paste Work
Reports That Build Themselves
Connect Your Tools, End Manual
Back-Office on Autopilot
Workflow Automation Agency
```
**Description:**
```
Your forms, CRM, sheets & invoices — connected so data moves itself. Free audit.
```

### AG4 — Local intent
**Keywords:** `"ai automation saudi arabia"  "automation agency khobar"  "ai automation riyadh"  "ai automation dubai"  "automation company gcc"`
**Headlines (add to AG1):**
```
AI Automation in Saudi Arabia
Al Khobar AI Automation Team
GCC AI Automation Agency
Local, Bilingual, On Your Time
```

---

## 4. Negative keywords (campaign-level — add all)
```
free  course  courses  tutorial  how to  diy  jobs  job  career  salary
internship  hiring  resume  cv  download  crack  open source  template
training  certification  what is  meaning  reddit  udemy  coursera  intern
freelancer fiverr  upwork  software free  no code free
```

## 5. Assets / extensions (add all — they lift CTR a lot)
- **Sitelinks:** `What we automate` `How it works` `Common questions` `WhatsApp us`
  → all point to the same page (anchor `/#` is fine) or the WhatsApp link for the last.
- **Callouts:** `Done-for-you` · `Bilingual عربي/EN` · `Free audit` · `Live in 2–4 weeks` · `ROI-priced`
- **Structured snippet** (Services): `Customer support AI, Data entry, Reporting, Workflow integration, Lead follow-up`
- **Call extension:** `+966 55 205 6371`
- **Business name / logo:** GLIO

## 6. Arabic ad (run as a second ad in each group — KSA converts on Arabic)
**Headlines:**
```
أتمتة الأعمال بالذكاء الاصطناعي
وفّر ساعات فريقك
تدقيق مجاني عبر واتساب
نبنيها ونشغّلها لك
دعم عملاء آلي ٢٤/٧
```
**Descriptions:**
```
نبني ونشغّل أتمتة ذكية لعملك: دعم العملاء، إدخال البيانات، التقارير. تدقيق مجاني.
فريق سعودي ثنائي اللغة. التسعير على أساس العائد. جاهز خلال أسابيع. راسلنا واتساب.
```

## 7. First 2 weeks — what to do
- Launch, **don't touch it 3–4 days** (let it learn).
- Watch **Search terms report** every 2–3 days → add junk as negatives.
- When a keyword spends ~2× your target cost-per-lead with 0 WhatsApp clicks → pause it.
- Aim to learn your **cost per WhatsApp lead**; once known, scale budget on the ad groups that produce them, cut the rest.
