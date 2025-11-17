# DGCP Verification Rules

Verification ensures that a DGCP record came from real life and  
real human work.

A valid DGCP record must include:

### 1. Original Timestamp  
Captured automatically by the device.

### 2. File Hash (SHA-256)
Ensures that the content has not been altered.

### 3. Source Information
Where the data was captured:
- device  
- location (optional)  
- context  

### 4. Description of Capture
Short explanation of what happened.

### 5. Storage Requirements
The record must be stored in:
- GitHub (mandatory)  
- IPFS (for selected files)  

### 6. No Rewrites Rule
Verification fails if:
- the file has been edited  
- metadata is missing  
- the timestamp is modified  
- the content is reconstructed later  

DGCP verification protects the integrity of real human work.
