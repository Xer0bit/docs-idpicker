---
title: "System Monitoring and Governance"
description: "How to check service health, read realtime logs, and manage free-use policies"
weight: 157
draft: false
---

For technical administrators, this section acts as your infrastructure dashboard. Here you can monitor server health, catch bugs as they happen, and control the financial levers of free usage.

---

## 1. Reviewing the Status Module

1. Open the **Status** page from the sidebar.
2. Review the core service health blocks (Database, API, AI Services, Storage).
3. If any component is flagged yellow (Degraded) or red (Offline), immediately cross-reference your infrastructure alerts.
4. The status page helps isolate whether a reported bug is a local user error or a widespread server outage.

---

## 2. Using Realtime Logs

When a user reports a persistent crash, the Realtime Logs are your best diagnostic tool.

1. Open the **Realtime Logs** module.
2. Click **Start Stream** to watch live events hit the backend in real-time.
3. Apply filters:
   - Set log level to `ERROR` or `FATAL` to strip out the noise.
   - Set the source filter if you are tracing a specific module (e.g., `stripe-webhook` or `ai-generation`).
4. Look for sudden bursts or cascading error statements. These can be exported and sent to your engineering team.

---

## 3. Free-Use Policy Management

If your platform offers a "freemium" tier, you need to govern exactly how much free API processing the average user can consume before hitting a paywall.

1. Open **Free Use Management**.
2. Review the current limit caps (e.g., *Max Free AI Chat Messages = 10*, *Max Free Reports = 1*).
3. Adjust the limits up or down depending on your current marketing strategy or token budget.
4. Click **Save**. The updated thresholds immediately apply to the gating logic on the student apps.

---

## 4. Certificates and Compliance Documents

1. Open the **Certificates** or **Application Documents** queue.
2. Review pending document validations submitted by users (e.g., proof of high school graduation or language proficiency).
3. Apply review decisions (Verify / Reject) based on your governance policy.
4. Add internal audit notes to every rejection for compliance tracking.

---

## Common Questions

| Situation | What to do |
|---|---|
| The Realtime Logs view is completely empty | Ensure you clicked "Start Stream". Also check if your exact filter combination is too restrictive (e.g., looking for FATAL logs on an entirely healthy system) |
| I see a massive spike in ERROR logs but the Status page says "Healthy" | A specific edge-case feature might be crashing (generating logs) without actually taking the core database offline. Investigate the log stack trace immediately |
| I updated the Free-Use limit but students say they are still blocked | Global platform settings often rely on multi-stage caching. Verify the environment variable propagated correctly, or wait 5 minutes for the cache TTL to expire |
