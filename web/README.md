# Web UIs

Each web UI implementation lives in its own directory, named after a Viking Age
artifact (`sunstone`, `runestone`, `seax`, `mjolnir`, …). Codenames don't age
the way "ui", "ui-new" or "ui-v2" do, and say nothing about the technology, so
implementations can come and go without renames.

| Codename | What                                        | Status  |
| -------- | ------------------------------------------- | ------- |
| sunstone | Vue 3 + Vuetify, the original OpenRelik UI  | default |

Code shared between UIs (API client, types, auth) goes into `shared/` once a
second implementation needs it. Released images keep a codename-free name
(ghcr.io/openrelik/openrelik-ui is the default UI), so deployments don't change
when the default does.
