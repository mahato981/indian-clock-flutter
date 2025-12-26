# GitHub Actions Workflows

## Build APK Workflow

This workflow automatically builds an APK file for the Indian Clock app whenever code is pushed to the main branch.

### How it works:

1. **Triggered by:** Push to main branch, pull requests, or manual trigger
2. **Actions performed:**
   - Checks out the code
   - Sets up Java 17 and Flutter 3.24.5
   - Gets dependencies
   - Analyzes code for issues
   - Builds release APK
   - Uploads APK as an artifact

### How to download the APK:

1. Go to the "Actions" tab in your GitHub repository
2. Click on the latest workflow run
3. Scroll down to "Artifacts" section
4. Download "indian-clock-app-release"
5. Extract the zip file to get your APK

### Creating a Release:

To create a GitHub Release with the APK:

```bash
git tag v1.0.0
git push origin v1.0.0
```

This will trigger the workflow and create a release with the APK attached.
