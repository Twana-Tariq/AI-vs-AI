# AI Content Detector – Key Actors

## 1. Identified Actors

| Actor | Type | Description |
|--------|-------|-------------|
| **End User (Content Verifier)** | Human User | Uploads or inputs text, image, audio, or video to check if it’s AI-generated. |
| **Administrator / Moderator** | Human User | Manages users, trending content, and system performance. |
| **External AI Detection Engine** | External System | Performs the actual AI detection and returns confidence scores. |

# AI Content Detector – Use Cases

## 1. Identified Actors

| Actor | Type | Description |
|--------|-------|-------------|
| **End User (Content Verifier)** | Human User | Uploads or inputs text, image, audio, or video to check if it’s AI-generated. |
| **Administrator / Moderator** | Human User | Manages users, trending content, and system performance. |
| **External AI Detection Engine** | External System | Performs the actual AI detection and returns confidence scores. |
| **AI Chat Assistant** | System Component | Explains detection results in detail and provides user guidance. |

---

## 2. Detailed Use Cases

### **UC-01: Detect AI-Generated Content**

| **Item** | **Description** |
|-----------|----------------|
| **Use Case ID** | UC-01 |
| **Use Case Name** | Detect AI-Generated Content |
| **Actors** | End User (Content Verifier), External AI Detection Engine |
| **Goal** | Allow the user to upload or input content (text, audio, image, video) to determine if it is AI-generated. |
| **Preconditions** | User is on the detection page and has selected a content type. |
| **Main Flow** | 1. User selects content type.<br>2. User uploads or enters the content.<br>3. System validates file format.<br>4. System sends content to AI Detection Engine.<br>5. Engine returns a detection result (AI probability, authenticity score).<br>6. System displays the detection result and confidence level to the user. |
| **Postconditions** | Detection result is stored in the database and can be viewed in user history. |
| **Alternate Flow(s)** | - If upload fails, user is prompted to retry.<br>- If detection engine is unavailable, a “Try again later” message is displayed. |

---

### **UC-02: View Trending Content Verification**

| **Item** | **Description** |
|-----------|----------------|
| **Use Case ID** | UC-02 |
| **Use Case Name** | View Trending Content Verification |
| **Actors** | End User, Administrator |
| **Goal** | Allow users to view trending content that has been verified for authenticity. |
| **Preconditions** | Trending data exists in the system (verified by admin or automated script). |
| **Main Flow** | 1. User navigates to the “Trending Verification” page.<br>2. System retrieves trending content items with verification data.<br>3. User views list with authenticity labels (AI-generated / Human-generated).<br>4. User can click on a content item for detailed detection report. |
| **Postconditions** | User views trending content and their verification details. |
| **Alternate Flow(s)** | - If no trending data available, system shows an empty state.<br>- If user is not logged in, only partial data (e.g., limited items) is shown. |

---

### **UC-03: Explain Detection Results**

| **Item** | **Description** |
|-----------|----------------|
| **Use Case ID** | UC-03 |
| **Use Case Name** | Explain Detection Results |
| **Actors** | End User, AI Chat Assistant |
| **Goal** | Provide a conversational explanation of detection results using the AI assistant. |
| **Preconditions** | Detection process is completed and results are available. |
| **Main Flow** | 1. User clicks “Explain Results.”<br>2. System sends the detection metadata to the AI Chat Assistant.<br>3. AI Assistant analyzes the data and provides a natural-language explanation (e.g., “This text shows high repetition and unnatural token distribution”).<br>4. User can ask follow-up questions for more context. |
| **Postconditions** | User gains understanding of how the AI determined the result. |
| **Alternate Flow(s)** | - If the AI Assistant is unavailable, the system displays a pre-generated static explanation. |

---

### **UC-04: Multi-Language Detection**

| **Item** | **Description** |
|-----------|----------------|
| **Use Case ID** | UC-04 |
| **Use Case Name** | Multi-Language Detection |
| **Actors** | End User, External AI Detection Engine |
| **Goal** | Enable detection of AI-generated content in multiple languages. |
| **Preconditions** | The user selects or uses a supported language. |
| **Main Flow** | 1. User selects language from the UI.<br>2. System localizes the interface and routes data to the appropriate AI Detection Engine model.<br>3. Engine performs multilingual analysis.<br>4. Detection results are returned and shown in the selected language. |
| **Postconditions** | User receives detection results localized in their chosen language. |
| **Alternate Flow(s)** | - If language is unsupported, system falls back to English.<br>- If translation module fails, an error is shown. |
