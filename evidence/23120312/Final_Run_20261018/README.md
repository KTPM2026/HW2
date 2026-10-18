# Final real test run — 18 October 2026

Native Android 16/API36 in Expo Go54.0.8 (not Expo Web); Web/Admin screenshots taken by Playwright. All PNGs are direct, unedited screen captures. API proof uses the official Swagger UI Execute button. No image generation was used. Passwords/JWTs are redacted from JSON. In the Swagger screenshot, the actual response pane is scrolled below the JWT line; the disposable password field remains visible.

A passive HTTP proxy records actual Mobile requests. Exactly one declared experiment D-C04 rewrites total_amount to1; all other requests pass unchanged. Original SUT business logic remains unchanged; only host/port adaptations are used. Original database hashes are preserved. Superseded automation errors are disclosed separately and are not product failures. The current test matrix has71 unique cases; repeated probes and reruns do not inflate the count.
