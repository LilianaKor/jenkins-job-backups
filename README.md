
<h1 align="center">🛡 Jenkins Job Backup</h1>

<p align="center">
  <img src="https://www.jenkins.io/images/logos/jenkins/jenkins.png" width="100" alt="Jenkins Logo"/>
</p>

<p align="center">
  Backup of <strong>jenkins-python-test</strong> multibranch pipeline<br/>
  ✅ Configured with Jenkinsfile<br/>
  🔄 Supports easy restore with builds & branches<br/>
</p>

---

## 🧾 What's Included

- ✅ Pipeline configuration (`config.xml`)
- 🌱 Branches (`main` and `dev`)
- 🧪 Build logs and workflow data
- 🔐 SCM hash and indexing state

---

## 🔄 Restore Instructions

To restore this job on a Jenkins instance:

```bash
# Step 1: Copy the project folder
cp -R jenkins-python-test ~/.jenkins/jobs/

# Step 2: Restart Jenkins
brew services restart jenkins-lts
```

> Jenkins will automatically detect and restore the job from backup.

---

## 📁 Backup Structure

```
jenkins-python-test/
├── branches/
│   ├── main/
│   └── dev/
├── indexing/
├── config.xml
└── state.xml
```

---

## 🔐 Private Use

This repository is private and intended for:

- Disaster recovery
- Migration between Jenkins setups
- Personal configuration archive

---

## ✨ Author

Made with 💚 by [Liliana](https://github.com/LilianaKor)
