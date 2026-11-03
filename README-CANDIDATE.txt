VALE Connect v0.9 production candidate — LOCAL PREPARATION ONLY

Based on development Build 8, a1878d175f6769e4a3d55112c48d8095a501facb.
Prepared for the existing https://valebrandworks.github.io/vale-connect/ address.
Uses the existing production public browser configuration and legacy local keys.
No deployment, migration, card import, publication, account or paid-plan change
has been authorized or performed.

This artifact must not be deployed or used to make production writes until the
user approves the specific deployment/migration/import actions. Offline tests use
synthetic storage and mock clients, without calling the production API.

Existing profiles and browser card/contacts are retained. Two new database
tables are required and currently absent; proposed SQL is a separate review
document, not an auto-run migration included in the runtime package.

Only the two reviewed real development cards are proposed for a later private
import. No card or contact data is embedded in this application package.
Synthetic profiles/connections are excluded. No automatic import/publication.

The existing development install (VALE Dev) remains a separate app. Following
an approved launch, install VALE Connect once from the production address.
Offline mode is a connection screen; cloud features require internet.

Keep the original v0.8.5 source recovery archive and private application-data
snapshot. User confirmed there are no legitimate contacts, including browser contacts;
no contact migration or contact-backup handoff is required. Do not clear
localStorage or reset accounts. No production credentials beyond the existing
public browser key are included.

Private owner release RC2: client account creation removed; interim owner-only
RLS is proposed separately. Server signup must be disabled and verified as the
first approved production step. This is not a deployed or fully implemented
Free/Pro/Business membership system. All synthetic data is excluded.
