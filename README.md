# sf-gha-install-package

GitHub action for å installere en pakke i en org ved bruk av sf cli.

Forutsetter at `jq` og `sf cli` er installert

## Bruk

<!-- Start usage -->
```yaml
- uses: navikt/sf-gha-install-package@<tag/sha>
  with:
    # Package version ID (04t...) or package alias
    # Required: true
    package-id: '04t...'
    
    # Org alias or username
    # Required: true
    target-org: 'my-org-alias'
    
    # Wait time for package install (minutes)
    # Required: false
    # Default: "10"
    install-wait: '10'

    # Publish wait time (minutes)
    # Required: false
    # Default: "10"
    publish-wait: '10'

    # Installation key for the package (if required)
    # Required: false
    # Default: ""
    package-key: ${{ secrets.PACKAGE_KEY }}
```
<!-- end usage -->

## Henvendelser

Spørsmål knyttet til koden eller prosjektet kan stilles som issues her på GitHub.

## For NAV-ansatte

Interne henvendelser kan sendes via Slack i kanalen #platforce.
