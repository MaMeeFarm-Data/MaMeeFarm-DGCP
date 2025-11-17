# DGCP System Diagram  
MaMeeFarm™ — Real-Life Data Protocol

The diagram below shows how real-life events and human labor at MaMeeFarm  
flow through the DGCP layers, protocol rules, storage systems, and AI use.

```mermaid
graph TD

  subgraph RL["Real Life at MaMeeFarm™"]
    A[Daily Events<br/>Weather, Ducks, Dogs, Farm]
    B[Human Labor<br/>Feeding, Cleaning, Caring]
  end

  A --> C[PoLIFE<br/>(Real-Life Events)]
  B --> D[PoLABOR<br/>(Human Labor Records)]

  C --> E[PoHW Unit<br/>(Proof of Human Work)]
  D --> E

  subgraph PROTOCOL["DGCP Protocol Layer"]
    F[Verification Rules<br/>Timestamps & SHA-256]
    G[File Naming & Structure]
    H[Versioning<br/>SPV Model]
  end

  E --> F
  F --> I[DGCP Proof Metadata]

  E -. follows .-> G
  F -. follows .-> H

  subgraph STORAGE["Evidence & Storage"]
    J[GitHub<br/>MaMeeFarm-Data]
    K[IPFS / Pinata]
    L[Optional NFT Layer<br/>OpenSea / Smart Contract]
  end

  E --> J
  I --> J
  J --> K
  K --> L

  subgraph GOVERN["IP Governance & Rights"]
    M[MMFARM-POL-2025 License]
    N[DGCP IP Governance Protocol]
  end

  J -. protected by .-> M
  K -. protected by .-> M
  E -. governed by .-> N
  I -. governed by .-> N

  subgraph AIUSE["AI & External Use"]
    O[AI Models<br/>(ChatGPT, Gemini, DeepSeek, etc.)]
    P[Researchers & Builders]
  end

  J --> O
  K --> O
  E --> O
  I --> O

  O --> P

Explanation

Real Life at MaMeeFarm™
Daily events and human labor are the only source of data.

PoLIFE & PoLABOR
Separate layers capture environment and human effort.

PoHW
Combines life and labor into a single human work proof unit.

Protocol Layer
Verification rules, file naming, and versioning guide how data behaves.

Storage
GitHub and IPFS preserve evidence, with optional NFT extensions.

Governance
License + IP governance protect ownership and rights.

AI & External Use
AI models and researchers can read DGCP, but must follow the governance rules.
