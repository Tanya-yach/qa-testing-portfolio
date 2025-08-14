# Luxor.cz Bug Reports
**Product Name:** Luxor (https://www.luxor.cz/)  
**Prepared by:** Tetiana Yachna  
**Date:** 14.07.2025  

---

## Bug #001: Email Validation Missing in Registration Form
**Severity:** Medium  
**Priority:** High  
**Environment:**  
- OS: Windows 11  
- Browser: Chrome 117  

**Description:**  
Email field does not show validation error when moving to another field.

**Steps to Reproduce:**
1. Open https://www.luxor.cz/
2. Go to registration form popup
3. Fill "E-mail" field with: `test_user@ua`
4. Click/tab to another field

**Expected Result:**  
Validation error appears: *"Zadejte prosím e-mail ve formátu 'xxx@xxx.cz'"*

**Actual Result:**  
No validation error appears

---

## Bug #002: Filter Reset Fails for Age Range
**Severity:** Medium  
**Priority:** Medium  
**Environment:**  
- OS: Windows 11  
- Browser: Chrome 117  

**Description:**  
"Zrušit filtry" button doesn't clear age range selection.

**Steps to Reproduce:**
1. Open https://www.luxor.cz/
2. Go to "Knihy" category
3. Apply filters:
   - Typ produktu: Knihy
   - Doporučený věk: 11-14 let
   - Jazyk: česky
4. Click "Zrušit filtry"

**Expected Result:**  
All filters reset completely

**Actual Result:**  
Age filter (11-14 let) remains applied

---

## Bug #003: Cart Counter Doesn't Update
**Severity:** Medium  
**Priority:** Medium  
**Environment:**  
- OS: Windows 11  
- Browser: Chrome 117  

**Description:**  
Cart icon counter fails to update when adding items.

**Steps to Reproduce:**
1. Open https://www.luxor.cz/
2. Add item to cart
3. Observe cart counter

**Expected Result:**  
Counter updates immediately (0 → 1)

**Actual Result:**  
Counter only updates after page refresh

---

## Bug #004: Incorrect Stock Status Display
**Severity:** High  
**Priority:** High  
**Environment:**  
- OS: Windows 11  
- Browser: Chrome 117  

**Description:**  
Product shows "SKLADEM" when it should be "NENI SKLADEM".

**Precondition:**  
Product ISBN-OUT-OF-STOCK-002 exists with "NENI SKLADEM" status

**Steps to Reproduce:**
1. Open product page for ISBN-OUT-OF-STOCK-002
2. Check stock status

**Expected Result:**  
Shows "NENI SKLADEM"

**Actual Result:**  
Shows "SKLADEM"

---

## Bug #005: Misaligned Mobile Buttons
**Severity:** Medium  
**Priority:** Low  
**Environment:**  
- Device: iPhone 12  
- OS: iOS 16.5  
- Browser: Chrome 117  
- Viewport: 390x844px  

**Description:**  
"Koupit" buttons appear at inconsistent heights.

**Steps to Reproduce:**
1. Open site on mobile
2. Scroll to product sections
3. Observe button alignment

**Expected Result:**  
Uniform button positioning

**Actual Result:**  
Buttons appear at varying heights