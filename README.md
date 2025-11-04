# folio-permissions-mappings

Copyright (C) 2024 The Open Library Foundation

This software is distributed under the terms of the Apache License, Version 2.0. See the file "[LICENSE](LICENSE)" for
more information.

## Description
This repository contains a file with mappings for permissions that cannot be processed automatically for various reasons. It requires manual mapping of type, resource, and action of capabilities. The file is used for processing capabilities in the `mod-roles-keycloak` module.

## Permission Mapping Governance

- **Do not remove** existing permission mappings from `mappings-overrides.json`.
- **Rationale:** External and internal consumers rely on this file; removals are breaking changes.

> ⚠️ **Important:** Direct removal from `mappings-overrides.json` breaks the system. Always use the module descriptor `replaces` mechanism for permission corrections.