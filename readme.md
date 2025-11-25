# VRChat Permission PSC Generator

This repository automatically generates a `Permissions.PSC` file for use with the permission package.

## Setup

1.  **Get your Group ID**: Find the ID of the VRChat group you want to track (e.g., `grp_xyz...`) and update the `groups` field in `.github/workflows/generate-psc.yml`.
2.  **Configure Secrets**: Go to `Settings` > `Secrets and variables` > `Actions` and add the following repository secrets:
    *   `VRCHAT_USERNAME`: Your VRChat login username.
    *   `VRCHAT_PASSWORD`: Your VRChat login password.
    *   `VRCHAT_2FA_KEY`: The secret key used to generate your 2FA codes (ensure you save this when enabling 2FA on VRChat).

## Output

Once the action runs, the file will appear in the `psc_output/` folder in this repository.