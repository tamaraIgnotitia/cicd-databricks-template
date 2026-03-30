# Databricks Platform Delivery Templates

Private repository — not for distribution. All contents are proprietary and confidential.

---

## What this is

This repository contains the reusable templates, configurations, and frameworks used to deliver the Databricks Platform Foundation Service. It is the canonical source for all delivery assets. Client engagements receive implementations built from these templates — not the templates themselves.

This repository predates and is independent of any client engagement.

---

## What this is not

This repository does not contain client-specific code, credentials, configuration, or data. No client work is stored here. Client deliverables live exclusively in the client's own repository.

---

## Structure

```
/cicd                   CICD pipeline templates (Databricks Asset Bundles)
  /dev-staging-prod     Standard three-environment DAB configuration
  /branching            Recommended branching strategy and PR templates

/unity-catalog          Unity Catalog setup templates
  /metastore            Metastore attachment and configuration
  /governance           Access groups, policies, service principals
  /schemas              Naming conventions and schema structure templates

/ingestion              Reference ingestion pipeline templates
  /api                  API source — batch and triggered
  /pdf                  PDF source — batch and triggered
  /storage              ADLS/blob storage source — batch and triggered
  /database             Database source — batch and triggered

/scd2                   SCD2 history tracking logic — reusable across source types

/runbook                Runbook template for client handover
  /operations           How to add schemas, sources, users, roll back deployments
  /onboarding           Client onboarding checklist template

/contracts              Statement of work and contract clause templates
  /dependencies         Client dependency schedule template
  /ip-clause            Internal use only clause for documentation and runbooks
```

---

## Usage

Each engagement begins by copying the relevant templates into the client's repository and adapting to their environment. Improvements discovered during delivery are back-ported to this repository after handover.

The client receives their adapted implementation. They do not receive access to this repository.

---

## Versioning

Templates are versioned by date of last update. When a Databricks platform update requires changes to the standard approach, templates are updated here first and the change is noted in the changelog.

---

## IP notice

All templates, frameworks, configurations, and documentation in this repository are original works authored by the repository owner. They are not derived from any client deliverable. Created: [DATE].

---

## Changelog

| Date | Change |
|------|--------|
| [DATE] | Repository created — initial structure |