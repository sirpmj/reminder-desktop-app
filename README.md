# Reminder & Follow-Up Desktop App

This is an Electron-based desktop version of the **Reminder & Follow-Up Dashboard**.

---

## How to Build a Portable EXE via GitHub Actions (No Windows Machine Needed)

### 1. Create a new GitHub repository
1. Go to [https://github.com/new](https://github.com/new)
2. Enter a repository name, e.g., `reminder-desktop-app`.
3. Choose **Private** (recommended) or **Public**.
4. Click **Create repository**.

### 2. Upload the project files
1. Unzip `reminder_app_portable_with_icon.zip` on your local machine.
2. Go to your new repo on GitHub.
3. Click **Add file → Upload files**.
4. Drag **all files and folders from inside the unzipped folder** (including `.github`, `index.html`, `package.json`, etc.) into the upload area.
5. Scroll down and click **Commit changes**.

### 3. Trigger the GitHub Actions build
1. Click the **Actions** tab in your repository.
2. Select **Build Windows EXE** from the list.
3. If asked to enable workflows, click **Enable workflow**.
4. Click the **Run workflow** button on the right.
5. In the dropdown, make sure branch = `main`, then click **Run workflow**.

### 4. Wait for the build to finish
- The workflow will appear in the list. Click it to see details.
- Wait until the yellow dot (in progress) turns green (success).

### 5. Download your portable EXE
1. On the successful run page, scroll to the **Artifacts** section.
2. Click the artifact name (`reminder-windows-installer`).
3. This will download a ZIP file — unzip it.
4. Inside you'll find your portable EXE file:
