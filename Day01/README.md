# Day 01 – Create Temporary Linux User

## 📜 Challenge Description
A developer named **kareem** requires temporary access to **App Server 1** in the Stratos Datacenter.
The account must expire automatically on **2024-04-15**.

---

## ⚙️ Requirements
- Username: `kareem` (lowercase)
- Expiry date: `2024-04-15`

---

## 🛠 Approach
1. SSH into App Server 1
2. Create user with expiry date
3. Verify expiry settings

---

## 💻 Commands Used
```bash
sudo useradd -e 2024-04-15 kareem
sudo chage -l kareem
