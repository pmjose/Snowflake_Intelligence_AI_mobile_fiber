# eSIM Implementation Guide
**Snowmobile Telco - Digital SIM Activation**

## Executive Summary

Snowmobile Telco's eSIM solution enables instant digital provisioning of mobile connectivity without physical SIM cards. With 48% of our new activations now via eSIM (up from 32% in 2024), we are leading the transition to digital-first mobile services for UK businesses.

---

## eSIM Overview

### What is eSIM?

eSIM (embedded SIM) is a digital SIM that allows activation of a mobile plan without a physical SIM card. The SIM is built into the device and can be programmed remotely.

### Benefits of eSIM

| Benefit | Description | Impact |
|---------|-------------|--------|
| Instant Activation | No waiting for physical SIM delivery | Hours → Minutes |
| Remote Provisioning | Activate anywhere in the world | Global deployment |
| Multiple Profiles | Switch between plans easily | Flexibility |
| Eco-Friendly | No plastic SIM cards | Sustainability |
| Secure | Tamper-resistant, encrypted | Enhanced security |
| Cost Savings | No shipping, no inventory | -40% logistics cost |

---

## Supported Devices

### Smartphones

| Manufacturer | Models | eSIM Support |
|--------------|--------|--------------|
| Apple | iPhone 16 series (Pro Max, Pro, Plus, Standard) | Full support |
| Apple | iPhone 15 series | Full support |
| Apple | iPhone SE (4th Gen) | Full support |
| Samsung | Galaxy S25 series (Ultra, +, Standard) | Full support |
| Samsung | Galaxy S24/S23 series | Full support |
| Samsung | Galaxy Z Fold6/Flip6 | Full support |
| Google | Pixel 9 series (Pro XL, Pro, Standard, 9a) | Full support |
| Google | Pixel 8/7 series | Full support |

### Tablets

| Manufacturer | Models | eSIM Support |
|--------------|--------|--------------|
| Apple | iPad Pro 13"/11" (M4) | Full support |
| Apple | iPad Air 13"/11" (M3) | Full support |
| Apple | iPad (11th Gen) | Full support |
| Apple | iPad mini (7th gen) | Full support |
| Samsung | Galaxy Tab S10 Ultra/+ | Full support |
| Samsung | Galaxy Tab S9 series | Full support |
| Microsoft | Surface Pro 11/10 | Full support |

### Wearables & IoT

| Category | Devices | eSIM Support |
|----------|---------|--------------|
| Smartwatches | Apple Watch Ultra 3, Series 10 | Full support |
| Smartwatches | Samsung Galaxy Watch 7 | Full support |
| Laptops | MacBook Pro (M4), ThinkPad X1 | Full support |
| IoT Modules | Quectel, Sierra Wireless 5G modules | eUICC support |

---

## Activation Process

### Consumer/SMB Activation

**Step 1: Order**
- Select eSIM-compatible plan
- Provide device IMEI/EID
- Complete order

**Step 2: Receive QR Code**
- Email with QR code (instant)
- SMS confirmation
- Portal access

**Step 3: Scan & Activate**
1. Go to device Settings
2. Select "Add Cellular Plan" / "Add eSIM"
3. Scan QR code
4. Confirm activation
5. Ready to use (typically <5 minutes)

### Enterprise Bulk Activation

**Option 1: QR Code Distribution**
- Bulk QR code generation
- Email to employees
- Self-service activation

**Option 2: MDM Push**
- Integrate with MDM (Intune, Jamf, VMware)
- Push eSIM profile remotely
- Zero-touch activation

**Option 3: SM-DP+ Direct**
- Direct server integration
- Automated provisioning
- API-driven activation

---

## Enterprise Features

### MDM Integration

| Platform | Integration Level | Features |
|----------|-------------------|----------|
| Microsoft Intune | Full | Remote provisioning, policy control |
| VMware Workspace ONE | Full | Zero-touch deployment |
| Jamf Pro | Full | Apple device management |
| MobileIron | Full | Cross-platform support |
| Hexnode | Partial | Basic provisioning |

### API Capabilities

```
eSIM Management API:
POST /esim/provision - Create new profile
GET /esim/{id}/status - Check activation status
POST /esim/{id}/activate - Activate profile
POST /esim/{id}/suspend - Suspend profile
DELETE /esim/{id} - Delete profile
GET /esim/bulk/{batch_id} - Bulk status check
```

### Security Features

| Feature | Description |
|---------|-------------|
| Profile Encryption | AES-256 encryption of profiles |
| Secure Download | TLS 1.3 protected transfer |
| Device Binding | Profile locked to device EID |
| Remote Lock | Lock/wipe eSIM remotely |
| Audit Logging | Complete activation audit trail |

---

## eSIM Tariffs

### Business eSIM Plans

| Plan | Data | Minutes | Price | eSIM Fee |
|------|------|---------|-------|----------|
| eSIM Essential 10GB | 10GB | Unlimited | £16/month | Free |
| eSIM Business 25GB | 25GB | Unlimited | £22/month | Free |
| eSIM Business 50GB | 50GB | Unlimited | £28/month | Free |
| eSIM Unlimited | Unlimited | Unlimited | £38/month | Free |
| eSIM 5G Premium | Unlimited 5G | Unlimited | £48/month | Free |

### Data-Only eSIM

| Plan | Data | Price | Use Case |
|------|------|-------|----------|
| eSIM Data 10GB | 10GB | £12/month | Tablets, laptops |
| eSIM Data 25GB | 25GB | £18/month | Heavy tablet users |
| eSIM Data 50GB | 50GB | £25/month | Mobile workers |
| eSIM Data Unlimited | Unlimited | £35/month | Power users |

### International eSIM

| Region | Data | Validity | Price |
|--------|------|----------|-------|
| EU Roaming | 15GB | 30 days | Included |
| USA | 10GB | 30 days | £25 |
| Global 50+ | 5GB | 30 days | £35 |
| Global 100+ | 10GB | 30 days | £55 |

---

## Implementation Guide

### Phase 1: Planning (Week 1-2)

**Tasks:**
- [ ] Audit device fleet for eSIM compatibility
- [ ] Review MDM capabilities
- [ ] Define activation workflow
- [ ] Identify pilot group
- [ ] Prepare communication plan

**Deliverables:**
- Device compatibility report
- Integration architecture
- Pilot plan

### Phase 2: Pilot (Week 3-4)

**Tasks:**
- [ ] Configure MDM integration
- [ ] Provision pilot group (25-50 users)
- [ ] Test activation process
- [ ] Gather feedback
- [ ] Resolve issues

**Success Criteria:**
- 95% successful activations
- <10 minute average activation time
- User satisfaction >4/5

### Phase 3: Rollout (Week 5-8)

**Tasks:**
- [ ] Communicate to all users
- [ ] Bulk provision eSIM profiles
- [ ] Support escalation process
- [ ] Monitor activation metrics
- [ ] Update documentation

**Rollout Options:**
| Approach | Timeline | Best For |
|----------|----------|----------|
| Big Bang | 1 week | Small orgs (<100 users) |
| Phased | 2-4 weeks | Medium orgs (100-500) |
| Rolling | 4-8 weeks | Large orgs (500+) |

---

## Troubleshooting

### Common Issues

| Issue | Cause | Solution |
|-------|-------|----------|
| QR code won't scan | Camera focus/lighting | Use well-lit area, clean lens |
| "Carrier not supported" | Device region lock | Contact support for unlock |
| Activation timeout | Network connectivity | Ensure WiFi connection |
| Profile won't download | Insufficient storage | Free up device space |
| No service after activation | Provisioning delay | Wait 5-10 minutes, restart |

### Support Contacts

| Issue Type | Contact | Response Time |
|------------|---------|---------------|
| Activation issues | esim-support@snowmobile.co.uk | 2 hours |
| MDM integration | enterprise@snowmobile.co.uk | 4 hours |
| API support | api-support@snowmobile.co.uk | 4 hours |
| Billing queries | billing@snowmobile.co.uk | 24 hours |

---

## Migration from Physical SIM

### Migration Process

1. **Backup** - Note existing number and settings
2. **Order eSIM** - Request eSIM replacement via portal
3. **Receive QR** - Instant delivery via email
4. **Activate** - Scan QR code on device
5. **Verify** - Test calls, data, SMS
6. **Recycle** - Return old SIM for recycling

### What Transfers

| Feature | Transfers to eSIM |
|---------|-------------------|
| Phone number | ✓ Yes |
| Data allowance | ✓ Yes |
| Contract terms | ✓ Yes |
| Voicemail | ✓ Yes |
| Call forwarding | ✓ Yes |
| Contacts | N/A (stored on device) |

---

## Sustainability Impact

### Environmental Benefits

| Metric | Traditional SIM | eSIM | Saving |
|--------|-----------------|------|--------|
| Plastic per SIM | 5g | 0g | 100% |
| Packaging | 15g card | Email | 100% |
| Shipping CO2 | 50g | 0g | 100% |
| Manufacturing CO2 | 120g | 0g | 100% |

### Annual Impact (Snowmobile Telco)

| Metric | 2024 Actual | 2025 YTD |
|--------|-------------|----------|
| eSIM activations | 45,000 | 68,000 |
| Plastic saved | 225 kg | 340 kg |
| CO2 saved | 7.6 tonnes | 11.5 tonnes |
| Shipping eliminated | 45,000 packages | 68,000 packages |

---

**Contact**: esim@snowmobile.co.uk  
**Date**: January 2025  
**Classification**: External

