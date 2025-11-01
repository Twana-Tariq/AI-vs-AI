### Role 2: Requirements Classification Specialist 

| ID | Requirement Description | Type | Level |
|----|--------------------------|------|-------|
| FR1 | Detect AI-generated text using RoBERTa model | Functional | System |
| FR2 | Detect AI-generated images using Deepfake model | Functional | System |
| FR3 | Detect AI-generated audio using wav2vec model | Functional | System |
| FR4 | Detect AI-generated video using GenConViT | Functional | System |
| FR5 | Detect AI-generated live stream content | Functional | System |
| FR6 | Allow users to upload different media files | Functional | User |
| FR7 | Display results (AI or Real) clearly to user | Functional | User |
| FR8 | Show trending AI-generated media awareness page | Functional | System |
| FR9 | Automatically update detection models | Functional | System |
| FR10 | Store detection results and logs in database | Functional | System |
| NFR1 | System must process detections within 5 seconds | Non-Functional | System |
| NFR2 | Maintain detection accuracy above 90% | Non-Functional | System |
| NFR3 | Must ensure user data privacy and security | Non-Functional | System |
| NFR4 | Interface should be user-friendly and intuitive | Non-Functional | User |
| NFR5 | System should scale to handle many users | Non-Functional | System |
| NFR6 | Support modularity for model replacement | Non-Functional | System |
| NFR7 | Work across platforms (web/mobile) | Non-Functional | System |
| NFR8 | Show error messages for unsupported files | Non-Functional | User |
| NFR9 | Multi-language support | Non-Functional | System |
| NFR10 |  AI chat assistant explaining results | Non-Functional | System |
### Role 5: Requirements prioritization analyst 
This section will prioritize all functional and non functional requirements according to project goals and feasability
The following table priortizes all requirements with its priority and justification 

| **ID** | **Requirement Description** | **Priority** | **Justification** |
|:--:|--------------------------------|:--:|--------------------|
| **FR1** | Detect AI-generated text using RoBERTa model | **M** | Core functionality of the system allows text analysis for AI content detection. |
| **FR2** | Detect AI-generated images using Deepfake model | **M** | Essential for identifying fake visual content and maintaining multi-media coverage. |
| **FR3** | Detect AI-generated audio using wav2vec model | **M** | Important for detecting AI-generated or deepfake voices directly supports project goal. |
| **FR4** | Detect AI-generated video using GenConViT | **M** | Required for complete detection coverage and ensures multi-modal accuracy. |
| **FR5** | Detect AI-generated live stream content | **N** | Valuable for real-time detection but not realistic at prototype stage. |
| **FR6** | Allow users to upload different media files | **M** | A must for users to interact with and test the detection system. |
| **FR7** | Display results (AI or Real) clearly to user | **M** | Ensures usability and helps users interpret detection outcomes. |
| **FR8** | Show trending AI-generated media awareness page | **N** | Adds awareness and engagement value but not required for the MVP. |
| **FR9** | Automatically update detection models | **M** | Maintains accuracy over time as AI models evolve.Supports system novelty |
| **FR10** | Store detection results and logs in database | **M** | Enables traceability, debugging, and evaluation of system performance. |
| **NFR1** | System must process detections within 5 seconds | **N** | Improves responsiveness and user experience but not essential for functionality. |
| **NFR2** | Maintain detection accuracy above 90 % | **M** | Needed for performance defines how successful the system is and it's credibility. |
| **NFR3** | Must ensure user data privacy and security | **M** | Builds trust and prevents misuse mandatory for ethical compliance. |
| **NFR4** | Interface should be user-friendly and intuitive | **N** | Improves accessibility and usability but not core to detection accuracy. |
| **NFR5** | System should scale to handle many users | **N** | Supports future growth but not important for first release. |
| **NFR6** | Support modularity for model replacement | **M** | Core system novelty allows updates without breaking architecture. |
| **NFR7** | Work across platforms (web / mobile) | **N** | Increases accessibility but not required for MVP. |
| **NFR8** | Show error messages for unsupported files | **N** | Enhances user experience but not system's core functions. |
| **NFR9** | Multi-language support | **S** | Adds unnecessary complexity and translation work at this stage. |
| **NFR10** | AI chat assistant explaining results | **S** | Interesting future feature but unrealistic considering our limited resources. |
