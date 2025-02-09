# IPFS Workshop 2 - Decentralization

This repository is part of an **IPFS Workshop** focused on decentralized file storage and website hosting using **IPFS (InterPlanetary File System)** and **Pinata**.

## 📌 Overview
This project demonstrates how to:
- Install and configure IPFS.
- Upload and manage files on IPFS.
- Deploy a static website to IPFS.
- Automate deployment using GitHub Actions and Pinata.

## 🛠️ Setup Instructions

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/YOUR_GITHUB_USERNAME/IPFS_workshop2_decentralization.git
cd IPFS_workshop2_decentralization
```

### 2️⃣ Install IPFS (Local Setup)
1. Download and install IPFS from: [https://docs.ipfs.tech/install/](https://docs.ipfs.tech/install/)
2. Initialize IPFS:
   ```sh
   ipfs init
   ipfs daemon &
   ```

### 3️⃣ Deploy Website to IPFS
- Ensure your website files are inside the **`website/`** directory.
- Manually add files to IPFS:
  ```sh
  ipfs add -r website/
  ```
- Copy the generated **CID** and access your website at:
  ```
  https://ipfs.io/ipfs/YOUR_CID
  ```

## 🚀 GitHub Actions Deployment
This repository is configured with a **GitHub Actions workflow** to automatically deploy the website to **IPFS via Pinata**.

### 🔧 Setup GitHub Secrets
To enable automated deployment, add the following **secrets** to your GitHub repository:
1. `PINATA_API_KEY` - Your Pinata API Key
2. `PINATA_API_SECRET` - Your Pinata Secret API Key

### 📜 Workflow Execution
The deployment workflow runs when changes are pushed to the `main` branch. You can trigger it manually from the **Actions tab**.

## 🔗 Useful Links
- [IPFS Documentation](https://docs.ipfs.tech/)
- [Pinata API Docs](https://docs.pinata.cloud/)
- [GitHub Actions Guide](https://docs.github.com/en/actions)

## 🤝 Contributing
Feel free to open **issues** or **pull requests** if you find any bugs or have suggestions.

---

**Created for IPFS Workshop 2 - Decentralization** 🚀

