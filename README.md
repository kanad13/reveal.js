# readme

- This repo is a forked copy of original [reveal.js](https://github.com/hakimel/reveal.js).
- I have made minor changes to it for my personal taste.

# dependabot alerts

These are the steps I use to fix Dependabot alert in this repo

- **Identify the Vulnerable Dependency**:
  - Review the Dependabot alert to identify which dependency and version are vulnerable.
- **Update Specific Vulnerable Dependencies**:
  - If the alert specifies a particular dependency, update it in the `package.json` to a non-vulnerable version as recommended by the alert.
- **Use `npm-check-updates` for Comprehensive Updates**:
  - Install `npm-check-updates` using: `npm install -g npm-check-updates`.
  - Run `npx npm-check-updates -u` to update all dependencies in the `package.json` to their latest versions, ignoring specified version ranges.
- **Install Updated Dependencies**:
  - Execute `npm install` to install the latest versions specified in your updated `package.json`. This will also update the `package-lock.json` file to reflect these changes.
- **Commit Changes**:
  - Commit the changes to the repository and go to the Insights section in GitHub for this repo and select Dependency Graph.
  - Click on Dependabot within the Dependency Graph section. And see if all vulnerabilities are taken care of.
