## 2025-02-21 - Dynamic Config Iteration Bottleneck
**Learning:** The application iterates through `CONFIG_LIST` for every URL check and site listing. This is O(N) for every request.
**Action:** Pre-compile regexes (implemented) and consider caching site lists if `CONFIG_LIST` is static.
