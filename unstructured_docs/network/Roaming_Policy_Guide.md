# International Roaming Policy Guide
**Snowmobile Telco - Business Roaming Services**

## Executive Summary

Snowmobile Telco provides comprehensive international roaming services for UK businesses. With coverage in 200+ destinations and EU roaming included at no extra cost, our customers stay connected wherever business takes them.

---

## EU Roaming (Roam Like at Home)

### Included Destinations

**Full EU Roaming (No Extra Cost):**
Austria, Belgium, Bulgaria, Croatia, Cyprus, Czech Republic, Denmark, Estonia, Finland, France, Germany, Greece, Hungary, Iceland, Ireland, Italy, Latvia, Liechtenstein, Lithuania, Luxembourg, Malta, Netherlands, Norway, Poland, Portugal, Romania, Slovakia, Slovenia, Spain, Sweden

### Fair Use Policy

| Plan Type | Data Allowance | Fair Use Limit |
|-----------|---------------|----------------|
| 5GB UK | 5GB | 5GB EU |
| 10GB UK | 10GB | 10GB EU |
| 25GB UK | 25GB | 15GB EU |
| 50GB UK | 50GB | 20GB EU |
| Unlimited UK | Unlimited | 25GB EU |

**After Fair Use Limit:**
- Additional data: £3.50/GB
- Calls/SMS: Continue at UK rates

### EU Roaming Terms

- Valid for temporary travel, not permanent use
- Maximum 4 months continuous roaming
- UK usage must exceed roaming usage over 4-month period
- Business plans exempt from domestic usage requirements

---

## International Roaming Zones

### Zone 1 - Popular Destinations

**Countries:** USA, Canada, Australia, New Zealand, Switzerland, Monaco, Andorra, San Marino, Vatican City

| Service | Pay Monthly | PAYG |
|---------|-------------|------|
| Calls made | £1.50/min | £2.00/min |
| Calls received | £0.75/min | £1.00/min |
| SMS sent | £0.40 | £0.50 |
| Data | £5.00/GB | £6.00/GB |

### Zone 2 - Extended International

**Countries:** Japan, South Korea, Singapore, Hong Kong, UAE, Israel, South Africa, Brazil, Mexico, Turkey

| Service | Pay Monthly | PAYG |
|---------|-------------|------|
| Calls made | £2.50/min | £3.00/min |
| Calls received | £1.25/min | £1.50/min |
| SMS sent | £0.50 | £0.60 |
| Data | £8.00/GB | £10.00/GB |

### Zone 3 - Rest of World

**Countries:** All other destinations including India, China, Russia, Africa (most), South America (most), Middle East (most)

| Service | Pay Monthly | PAYG |
|---------|-------------|------|
| Calls made | £3.50/min | £4.50/min |
| Calls received | £1.75/min | £2.25/min |
| SMS sent | £0.60 | £0.75 |
| Data | £12.00/GB | £15.00/GB |

---

## Roaming Bundles

### Travel Data Passes

| Pass | Data | Validity | Destinations | Price |
|------|------|----------|--------------|-------|
| Europe Plus | 5GB | 30 days | EU + Switzerland | £15 |
| USA & Canada | 5GB | 30 days | USA, Canada | £20 |
| World Traveller | 3GB | 30 days | 50+ countries | £30 |
| Global Business | 10GB | 30 days | 100+ countries | £55 |
| Unlimited EU | Unlimited | 30 days | EU only | £35 |

### Enterprise Travel Solutions

| Solution | Description | Pricing |
|----------|-------------|---------|
| Corporate Pool | Shared data for travelling employees | From £500/month |
| Global SIM | Single SIM, worldwide coverage | From £45/month |
| Local Breakout | Local rates in key markets | Custom |
| Private APN | Secure roaming connection | £200/month + usage |

---

## Cruise & Flight Roaming

### Maritime Roaming

**Cruise Ships:**
- Coverage via satellite on most major cruise lines
- Higher rates apply (£5/MB typical)
- Recommend: Purchase ship WiFi + use WiFi calling

| Service | Rate |
|---------|------|
| Calls | £6.00/min |
| Data | £5.00/MB |
| SMS | £0.75 |

### In-Flight Connectivity

**Airlines with Connectivity:**
- British Airways, Virgin Atlantic, Emirates, Lufthansa, etc.

| Service | Rate |
|---------|------|
| Data | £10.00/MB |
| SMS | £0.50 |

**Recommendation:** Use airline WiFi with WiFi calling enabled

---

## WiFi Calling

### Using WiFi Calling Abroad

WiFi Calling allows you to make and receive calls over WiFi as if you were in the UK:

**Benefits:**
- UK rates for calls and texts
- No roaming charges
- Works anywhere with WiFi
- Crystal clear quality

**Setup:**
1. Enable WiFi Calling in device settings
2. Connect to WiFi network
3. Make calls as normal
4. Charged at UK rates

**Supported Devices:**
- All iPhones (6s and later)
- Samsung Galaxy S8 and later
- Google Pixel 3 and later
- Most Android devices (2019+)

---

## Roaming Spend Controls

### Automatic Protections

| Control | Default | Customisable |
|---------|---------|--------------|
| Data roaming cap | £45/month | Yes |
| Bill shock alert | £35/month | Yes |
| Roaming disabled | No | Yes |
| Zone restrictions | None | Yes |

### Setting Spend Limits

**Via Portal:**
1. Log into Business Portal
2. Navigate to "Roaming Controls"
3. Set desired limit (£0-1000)
4. Apply to individual or all lines

**Via API:**
```
POST /lines/{msisdn}/roaming-cap
{
  "amount": 50.00,
  "currency": "GBP",
  "action": "suspend" // or "notify"
}
```

---

## Emergency Roaming

### Emergency Services Abroad

**EU (112):**
- Works in all EU countries
- GPS location shared with services
- Free to call

**USA (911):**
- Works on all networks
- Location shared where available
- Free to call

**Other Countries:**
- Local emergency numbers apply
- See country guide for specific numbers

### Lost/Stolen Device Abroad

**Immediate Actions:**
1. Call +44 800 123 4567 (24/7 support)
2. Report device stolen
3. Request SIM block
4. Request IMEI block

**Next Steps:**
- Arrange replacement SIM to hotel/office
- eSIM activation available (if device compatible)
- Insurance claim if applicable

---

## Business Travel Tips

### Before You Travel

- [ ] Check destination coverage
- [ ] Enable WiFi Calling
- [ ] Download offline maps
- [ ] Purchase data pass if needed
- [ ] Note emergency contacts
- [ ] Enable spend alerts

### During Travel

- [ ] Use WiFi where possible
- [ ] Disable auto-updates on roaming
- [ ] Use data saver mode
- [ ] Monitor usage in portal/app
- [ ] Report any issues promptly

### Popular Destination Guides

| Country | Best Option | Notes |
|---------|-------------|-------|
| USA | Zone 1 pass or WiFi | Excellent coverage |
| France | EU roaming (free) | Use as UK |
| Germany | EU roaming (free) | Use as UK |
| UAE | Zone 2 pass | High local rates |
| China | Zone 3 or local SIM | Great Firewall affects apps |
| India | Zone 3 or local SIM | Good local options |

---

## Roaming Support

### 24/7 Roaming Helpline

**From UK:** 0800 123 4567  
**From Abroad:** +44 800 123 4567  
**WhatsApp:** +44 7XXX XXXXXX

### Roaming Issues Resolution

| Issue | Resolution Time | Credit Policy |
|-------|-----------------|---------------|
| No service | Immediate support | Pro-rata credit if >4hrs |
| Incorrect charging | 48 hours | Full refund if error |
| Bill shock | 24 hours | Case-by-case review |
| Emergency | Immediate | Priority handling |

---

**Contact**: roaming@snowmobile.co.uk  
**Date**: January 2025  
**Classification**: External

