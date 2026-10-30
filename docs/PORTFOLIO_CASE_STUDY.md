# Portfolio case study

The edited case study from the design lab is available at `/showcase`; the operational dashboard remains at `/`. Run `npm start` to serve both.

The page has a brief introduction followed by six interactive reconstructions. Each case keeps its source documentation, outcome, limitations, and expandable technical metadata together. Fonts and the project mark are served locally under the existing content security policy. See `Manrope-OFL.txt` for the font license.

Scenario fixtures describe documented tests rather than current local events. They never invoke tools, issue approvals, generate audit records, or run native diagnostics. The native case refers to a separate signed diagnostic build, not a fresh test of the installed worker. The approval fixture does not include note content.

The integration adds seven fixed static GET routes and a dashboard link. It does not change the policy engine, approval handlers, audit storage, MCP gateway, or native worker. Source links use the canonical mcp-approval-gateway repository name.

Verification: `npm test` includes scenario scope and HTTP checks for the showcase resources, TrueType font bytes, dashboard link, restricted paths, and lack of audit writes. Browser checks cover case and stage selection, deep links, history navigation, keyboard disclosure, responsive layout, and the distinction between reconstructed cases and live controls.
