# Setup Instructions

This folder is ready to use as the `leonlimwf/leonlimwf` GitHub profile repository.

## Repository structure

```text
leonlimwf/
├── README.md
└── .github/
    └── workflows/
        ├── profile-3d.yml
        └── snake.yml
```

## Install

1. Open the GitHub repository named exactly `leonlimwf/leonlimwf`.
2. Upload the contents of this folder while preserving the `.github/workflows` directories.
3. Commit the files to the repository's default branch.
4. Open **Actions** and manually run:
   - **Generate 3D contribution calendar**
   - **Generate contribution snake**
5. Refresh the profile after both workflows succeed.

The 3D calendar is committed into:

```text
profile-3d-contrib/profile-green-animate.svg
```

The snake workflow publishes its SVG files to an `output` branch.

## Required workflow permissions

The workflow files declare:

```yaml
permissions:
  contents: write
```

For most repositories, this is sufficient. If GitHub blocks the commit or output branch:

1. Open the profile repository.
2. Go to **Settings → Actions → General**.
3. Under **Workflow permissions**, select **Read and write permissions**.
4. Save, then run both workflows again.

## Private contribution visibility

GitHub profile settings control whether private contribution counts appear publicly. Enabling private contributions does not expose private repository names or content.

## Optional upgrades

Add product screenshots later under an `assets/` folder and place them above each featured project's description. A short compressed GIF or WebP of OrderEase is more persuasive than adding more generic statistics widgets.