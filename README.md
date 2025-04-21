
# 🛡 Jenkins Job Backup

This repository contains a backup of the `jenkins-python-test` multibranch pipeline project from Jenkins, including:

- ✅ Pipeline configuration (`config.xml`)
- 🌱 Branches (`main` and `dev`)
- 📦 Build logs and workflow data
- 🔐 SCM hash and indexing state

---

## 🔄 How to restore

To restore this project into Jenkins:

1. Copy the folder to your Jenkins jobs directory:

```bash
cp -R jenkins-python-test ~/.jenkins/jobs/
```

2. Restart Jenkins to reload the configuration:

```bash
brew services restart jenkins-lts
```

Jenkins will automatically detect and restore the project.

---

## 📁 Structure

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

## 🔒 Private Use

This repository is private and intended only for backup, recovery, or migration of Jenkins jobs.
