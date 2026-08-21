# Setup

This package is designed for the GitHub profile repository:

`Subhajit054/Subhajit054`

## 1. Replace the profile repository files

Upload/replace:

- `README.md`
- `assets/evolution.svg`
- `assets/skills.svg`
- `assets/projects.svg`
- `assets/engineering.svg`
- `profile/stats.svg`
- `profile/top-langs.svg`
- `.github/workflows/update-profile-stats.yml`

## 2. Commit and push

Once the files are in the profile repository, GitHub will render the local SVG assets immediately.

## 3. Enable the telemetry workflow

Open:

**GitHub → your profile repository → Actions → Update profile telemetry → Run workflow**

The workflow also runs automatically once per day.

It generates the stats cards directly into `profile/`, so the README does not depend on the public `github-readme-stats.vercel.app` service.

## 4. If the workflow cannot push

The workflow already requests:

```yaml
permissions:
  contents: write
```

If your repository has restrictive organization/repository policies, allow GitHub Actions to write repository contents.

## 5. Why the old images were broken

The old README referenced:

- `./assets/skills.svg`
- `./assets/projects.svg`

but those files were missing from the package/repository.

The old GitHub telemetry referenced public third-party generated-image endpoints. Those endpoints can rate-limit or go offline. The new version generates and stores the cards in your own repository instead.
