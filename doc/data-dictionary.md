# Data Dictionary (SharePoint List: tblInventory)

| Field | Type | Required | Example | Notes |
|------|------|----------|---------|------|
| ItemName | Text | Yes | "Roche Calibrator" | Standardised naming recommended |
| HIMF | Text | Yes | "HIMF-123456" | Unique identifier used for traceability |
| LotNumber | Text | Yes | "L2026A01" | Manufacturer lot |
| Supplier | Choice/Text | Yes | "Roche" | Prefer controlled list |
| Category | Choice | Yes | "Biochemistry" | Used for filtering/reporting |
| ReceivedDate | Date | Yes | 2026-02-23 | Date stock received |
| ExpiryDate | Date | Yes | 2026-09-30 | Critical for expiry logic |
| Site | Choice/Text | Recommended | "Tumut" | Enables multi-lab scalability |
| Quantity | Number | Optional | 2 | Units received |
| Status | Choice | Optional | "Active" | Can be calculated or manual |
