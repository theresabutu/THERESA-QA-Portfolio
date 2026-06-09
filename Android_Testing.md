# ✅ Device Adaptivity – Android Test Cases

---

> ⚠️ **Note**: These test cases are examples. Real-world implementations may differ by device matrix, OS version, or QA workflow.

---

## 🎯 Scope

These Android test cases cover:

- 📐 Layout responsiveness across screen sizes and orientations  
- 🧠 System-level font scaling and accessibility modes  
- 🔄 Split-screen and multitasking behavior  
- 📲 Compatibility with foldable and notch devices  
- 🌙 Dark mode and high-contrast UI validation

---

### ⛔ Out of Scope

- **iOS-specific layout behavior** – see [iOS_Testing.md](./iOS_Testing.md)  

---

## 📱 TC-ADAPT-AND-001 – Layout on various Android screen sizes

**Title:** Layout rendering on small, medium, and large Android devices  
**Section:** Device Adaptivity – Android  
**Template:** Steps + Results  
**Type:** Functional  
**Priority:** High  
**Status:** Approved  
**Defects:** —  
**Execution Status:** Passed  
**Automation:** Manual  
**Assigned To:** QA Engineer  
**Estimate:** 3m  
**References:** REQ-ADAPT-001  
**Preconditions:** App installed; scaling options set to default

**Steps and Results:**

| Step | Action                            | Expected Result                               |
|------|-----------------------------------|-----------------------------------------------|
| 1    | Launch app on 4.5" Android phone  | Layout appears without cutoff or overlap      |
| 2    | Launch app on 6" Android device   | Layout scales properly and centers            |
| 3    | Launch app on 10" tablet          | UI adapts with consistent spacing and visuals |

**Postconditions:** Layout verified across target screen sizes  
**General Expected Result:** Responsive UI across device sizes

---

## 📱 TC-ADAPT-AND-002 – Orientation change handling

**Title:** Validate layout during orientation changes  
**Section:** Device Adaptivity – Android  
**Template:** Steps + Results  
**Type:** Functional  
**Priority:** Medium  
**Status:** Approved  
**Defects:** —  
**Execution Status:** Passed  
**Automation:** Manual  
**Assigned To:** QA Engineer  
**Estimate:** 2m  
**References:** REQ-ADAPT-002  
**Preconditions:** App installed; device supports rotation

**Steps and Results:**

| Step | Action                          | Expected Result                                 |
|------|---------------------------------|-------------------------------------------------|
| 1    | Launch app in portrait mode     | Layout renders correctly                        |
| 2    | Rotate device to landscape      | Layout reflows without distortion               |
| 3    | Rotate back to portrait         | Layout returns to original state seamlessly     |

**Postconditions:** Layout remains stable across orientation changes  
**General Expected Result:** UI adapts smoothly to rotation

---

## 📱 TC-ADAPT-AND-003 – Font scaling via Accessibility

**Title:** Validate layout with system font scaling  
**Section:** Device Adaptivity – Android  
**Template:** Steps + Results  
**Type:** Accessibility  
**Priority:** Medium  
**Status:** Approved  
**Defects:** —  
**Execution Status:** Passed  
**Automation:** Manual  
**Assigned To:** QA Engineer  
**Estimate:** 2m  
**References:** REQ-ADAPT-003  
**Preconditions:** Font scaling enabled in system settings

**Steps and Results:**

| Step | Action                                | Expected Result                                 |
|------|---------------------------------------|-------------------------------------------------|
| 1    | Enable large font size in settings    | System font size increases                      |
| 2    | Launch app                            | Text scales without breaking layout             |
| 3    | Navigate through screens              | All content remains readable and accessible     |

**Postconditions:** Layout supports accessibility scaling  
**General Expected Result:** UI remains usable with large fonts

---

## 📱 TC-ADAPT-AND-004 – Split-screen multitasking behavior

**Title:** Validate layout in split-screen mode  
**Section:** Device Adaptivity – Android  
**Template:** Steps + Results  
**Type:** Usability  
**Priority:** Medium  
**Status:** Approved  
**Defects:** —  
**Execution Status:** Passed  
**Automation:** Manual  
**Assigned To:** QA Engineer  
**Estimate:** 2m  
**References:** REQ-ADAPT-004  
**Preconditions:** Device supports split-screen; app launched

**Steps and Results:**

| Step | Action                              | Expected Result                                 |
|------|-------------------------------------|-------------------------------------------------|
| 1    | Enter split-screen with another app | Layout adjusts to reduced width                 |
| 2    | Interact with app in split mode     | No overlap or cutoff; UI remains functional     |
| 3    | Exit split-screen                   | Layout returns to full-screen state             |

**Postconditions:** App remains usable in multitasking mode  
**General Expected Result:** UI adapts to split-screen constraints

---

## 📱 TC-ADAPT-AND-005 – Foldable device layout integrity

**Title:** Validate layout on foldable Android devices  
**Section:** Device Adaptivity – Android  
**Template:** Steps + Results  
**Type:** Compatibility  
**Priority:** Medium  
**Status:** Approved  
**Defects:** —  
**Execution Status:** Passed  
**Automation:** Manual  
**Assigned To:** QA Engineer  
**Estimate:** 3m  
**References:** REQ-ADAPT-005  
**Preconditions:** App installed on foldable device

**Steps and Results:**

| Step | Action                          | Expected Result                                 |
|------|---------------------------------|-------------------------------------------------|
| 1    | Launch app in folded state      | Layout fits compact screen                      |
| 2    | Unfold device                   | Layout expands and reflows correctly            |
| 3    | Fold back                       | UI returns to compact layout without glitches   |

**Postconditions:** Layout verified across fold states  
**General Expected Result:** Seamless transition between folded/unfolded

---

## 📱 TC-ADAPT-AND-006 – Dark mode and contrast validation

**Title:** Validate UI in dark mode and high contrast  
**Section:** Device Adaptivity – Android  
**Template:** Steps + Results  
**Type:** Accessibility  
**Priority:** Medium  
**Status:** Approved  
**Defects:** —  
**Execution Status:** Passed  
**Automation:** Manual  
**Assigned To:** QA Engineer  
**Estimate:** 2m  
**References:** REQ-ADAPT-006  
**Preconditions:** Dark mode enabled in system settings

**Steps and Results:**

| Step | Action                          | Expected Result                                 |
|------|---------------------------------|-------------------------------------------------|
| 1    | Enable dark mode                | System switches to dark theme                   |
| 2    | Launch app                      | UI elements adapt to dark background            |
| 3    | Enable high contrast mode       | Text and icons remain visible and readable      |

**Postconditions:** UI remains accessible in dark/high-contrast modes  
**General Expected Result:** Visual clarity preserved across themes
