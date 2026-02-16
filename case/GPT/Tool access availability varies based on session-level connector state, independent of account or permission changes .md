Case ID:
CASE-2026-02-16-TOOL-ACCESS-SESSION-BOUNDARY

Title:
Tool access availability varies based on session-level connector state, independent of account or permission changes


Summary:

[JP]
LLMのGoogle CalendarおよびGmailへのアクセス可否は、
ユーザーアカウントや権限設定が同一であっても、
セッション単位で変動することが観測された。

アクセス可否は、コネクタのセッション接続状態に依存し、
LLM自体の能力やユーザー権限の変更とは無関係である。

[EN]
Access availability to Google Calendar and Gmail varies per session,
even when user account and permission settings remain identical.

Availability is dependent on connector session state,
not on LLM capability changes or user permission modifications.


Environment:

Device:
iOS native ChatGPT app

Account:
same account across all tests

Permission:
no permission change between successful and unsuccessful attempts

External connectors:
Google Calendar connector
Gmail connector


Observed States:

State A — Connector active (success):

Timestamp:
2026-02-10 06:55 JST

Results:
Gmail: accessible
Google Calendar: accessible

Behavior:
LLM successfully retrieved external tool data


State B — Connector inactive (blocked):

Timestamp:
2026-02-16 09:20 JST

Results:
Gmail: inaccessible
Google Calendar: inaccessible

Behavior:
LLM unable to retrieve external tool data
No permission prompt shown
No error message shown


Control Variables:

Constant:
Account
Device
User permissions
User identity

Variable:
Session state
Connector activation state


Key Observation:

[JP]
ツールアクセスはユーザー権限ではなく、
セッション単位のコネクタ接続状態によって制御されている。

[EN]
Tool access is governed by session-level connector activation,
not by user permission state.


Mechanism Model:

User Account Layer
    ↓
Connector Authorization Layer
    ↓
Session Connector Activation Layer   ← observed control boundary
    ↓
LLM Tool Invocation Layer
    ↓
External Tool Access


Conclusion:

[JP]
ツールアクセス能力は恒久的なLLM能力ではなく、
セッション単位で付与される一時的能力である。

[EN]
Tool access capability is not a permanent LLM ability,
but a temporary capability granted per session.


Classification:

Type:
Capability Boundary Case

Severity:
None (expected behavior)

Reproducibility:
High

Confidence Level:
High


Implications:

[JP]
LLMの能力は固定ではなく、
セッション構造によって動的に変化することが確認された。

[EN]
LLM capability is not static,
but dynamically varies based on session structure.


Recommended Documentation Placement:

/cases/case-tool-access-session-boundary.md