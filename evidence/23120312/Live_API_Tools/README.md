# Live API tool screenshots 18 October 2026

These 21 PNGs are direct, unedited Playwright screenshots of real Swagger UI 5.33.3 and Datasette 0.65.5 pages. Swagger UI's Execute button sent requests directly to an isolated EShop backend (source 85af3ba); Datasette executed actual read-only SQL against that backend's SQLite file. No response interception, mocking or image generation was used.

Seven previously reported defect groups were reproduced. The actual catalog product price was 30000000; the forged-total cart had quantity 2, total 60000000. The original 14 October fixture values and test matrix have not been overwritten. This is a separate 18 October reproduction.

The Swagger UI OpenAPI descriptions define request inputs only. The generated cURL preview is hidden using CSS to keep JWT values out of public pictures. Request URL, HTTP status, server response body, and SQL results are unchanged. Test credentials are redacted in the downloadable JSON. No credentials for real accounts were used.

`Live_Tool_Reproduction.json` records requests, SQL, timestamps, fixture IDs, assertions and screenshot hashes. For the moving lock countdown, the Datasette HTML page and the separate JSON query execute milliseconds apart; their remaining-seconds values may differ slightly. Both show approximately 180 seconds, compared with the 30-second requirement.

The first automation attempt hit a strict-locator error after the API returned 401; the locator was corrected and the final reproduction completed all seven groups. That harness error is not a product bug. Original databases were hash-checked and remained unchanged. Mobile was not run.
