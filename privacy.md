# Privacy Policy
  
  **Effective date:** 2026-06-16
  **Last updated:** 2026-06-16

  This Privacy Policy describes how Remember4Me ("we", "us", "the app") handles
  information when you use the Remember4Me mobile application. Remember4Me is
  operated by Renu Khandelwal ("the developer").

  ## Quick summary
  
  Remember4Me is designed to be **end-to-end encrypted**. Your notes, document
  contents, tags, and document files are encrypted on your device using a key
  that only you control. We — the developer, our servers, and our cloud
  providers — cannot read your notes, documents, or any content you save.
  What we can see is limited to account identifiers (your email from Sign in
  with Apple or Sign in with Google), bookkeeping metadata (how many bytes you
  have synced, request counts for rate limiting), and the requests our AI
  features send to Anthropic for tag suggestion and summarization.

  ## What information we collect

  ### Account identity
  When you sign in, we receive from your chosen identity provider:
  - **Sign in with Apple:** your name (if you choose to share it) and a stable
    Apple identifier. Apple may also send a private relay email address that
    forwards to your real email; we never see your real address in this case.
  - **Sign in with Google:** your name, email, and a stable Google identifier.

  We store these identifiers to recognize you on future sign-ins. We do not
  share them with third parties for marketing.

  ### Rate-limiting identifier
  On first launch, the app generates a random per-install UUID and stores it
  in your device's secure storage. This UUID is sent with each request to
  our backend for rate-limiting purposes and is not linked to your account.

  ### Encrypted backups (only if you enable cloud sync)
  If you enable cloud sync (off by default), the app uploads an **encrypted**
  SQLite snapshot of your data to our backend infrastructure (Cloudflare R2).
  We can see the size of the file and when it was last updated, but the
  content is encrypted with a key derived from your passphrase. We do not
  know your passphrase and cannot decrypt this file.

  If you connect Google Drive for per-file backup (off by default, opt-in
  per document), encrypted file blobs are uploaded to your own Google Drive
  account in a folder named "Remember4Me". We do not have access to your
  Google Drive contents; only the app, signed in as you, does.

  ### AI feature requests
  When you use AI features (automatic tag suggestion, summarization), the
  relevant text is sent through our backend to **Anthropic** (the operator of
  Claude AI) for processing. Anthropic's handling of these requests is
  governed by Anthropic's own privacy policy
  (https://www.anthropic.com/legal/privacy). At the time of writing, Anthropic
  does not retain API request content for training.

  We cache successful AI responses on your device (encrypted) so that
  re-tagging the same content does not re-send it.

  ### What we do NOT collect
  - We do not collect analytics or usage telemetry.
  - We do not include third-party advertising or ad-tracking networks.
  - We do not sell, rent, or trade your information.
  - We do not use cookies (native app, no web tracking).
  - We do not access your contacts, location, calendar, microphone, or other
    device data, except when you explicitly grant permission for a feature
    (e.g., camera for document scanning, photo library for image import,
    notifications for reminders).

  ## How we use the information we collect
  
  - **Account identifiers**: to authenticate you on each launch and link your
    device to your encrypted backups.
  - **Rate-limiting UUID**: to prevent abuse of our backend by capping
    per-install request rates.
  - **Encrypted backup bookkeeping** (size, last update time): to enforce
    storage quotas and surface backup status to you in the app.
  - **AI requests**: to provide the tag-suggestion and summarization features.

  ## Third parties

  We use the following service providers:
  
  | Provider | Purpose | What they receive |
  |---|---|---|
  | **Apple** | Sign in with Apple | Their standard auth flow |
  | **Google** | Sign in with Google; optional Drive backup of encrypted file blobs | Auth flow;
  encrypted blobs in your own Drive |
  | **Anthropic** | AI text processing for tags and summaries | The relevant text from your in-app
  actions |
  | **Cloudflare** | Hosting our backend Worker, encrypted SQLite snapshot storage (R2), and
  rate-limit state | Encrypted backups + bookkeeping; never plaintext |

  We do not share your data with anyone else for any purpose.
  
  ## Data retention and deletion

  - Data on your device is retained until you delete it from the app or
    uninstall the app.
  - Encrypted backups in our infrastructure are retained until you delete
    your account in the app, which triggers a server-side wipe of your
    encrypted snapshot and metadata.
  - You can request manual deletion at any time by emailing the contact
    address below.

  ## Your rights

  Depending on your region (EU, UK, California, etc.), you may have the
  right to:
  - Access the personal data we hold about you.
  - Request correction or deletion.
  - Withdraw consent for processing.
  - Lodge a complaint with a supervisory authority.

  To exercise any of these rights, contact us at the email below. Because
  your content is end-to-end encrypted with your key, we cannot provide
  you with the content of your notes or documents — only you can read those
  on your device.

  ## Children's privacy

  Remember4Me is not directed to children under 13 (or under 16 in the
  European Economic Area). We do not knowingly collect information from
  children. If you believe a child has used the app, please contact us so
  we can delete their account.

  ## Security
  
  We use platform-standard encryption (AES-256 with hardware-backed keys
  on iOS Secure Enclave and Android Keystore where available) to protect
  content on your device. Cloud backups are encrypted before they leave
  your device. No system is perfectly secure, but we have designed
  Remember4Me so that we cannot read your content even if our servers are
  compromised.

  ## Changes to this policy
  
  If we make material changes, we will update the "Last updated" date at
  the top of this page and, where appropriate, notify you in the app
  before the change takes effect.

  ## Contact
  
  For privacy questions, data requests, or to exercise the rights
  described above:

  **Email:** renu.k.rjam.ai@gmail.com

  **Developer of record:** Renu Khandelwal
