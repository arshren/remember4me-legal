 # Data Deletion Request — Remember4Me
  
  If you would like Remember4Me to delete your data, you have two options:

  ## Option 1 — Delete your data inside the app (fastest)
  
  Open Remember4Me on your phone and use any of these in-app actions:

  - **Delete a single document**: open the document, tap the Delete button in the action row at the
  bottom.
  - **Delete a memory (bundle)**: open the memory, tap Delete.
  - **Delete your entire account and all backups**: go to Settings → Account → Delete account. This
  wipes:
    - All local data on your device
    - Your encrypted backup in our cloud infrastructure (Cloudflare R2)
    - Your per-doc encrypted files in your Google Drive's `Remember4Me` folder

  In-app deletion is immediate and irreversible.

  ## Option 2 — Email us
  
  If you no longer have access to your phone or prefer to make a written
  request (for example, to exercise a right under GDPR or CCPA), send an
  email to:
  
  **renu.k.rjam.ai@gmail.com**

  Please include:
  - The email address you used to sign in (Apple Sign In or Google Sign In)
  - A statement of what you would like deleted (everything, a specific
    document, etc.)

  We will process the request within 30 days.

  ## What we delete

  - Account identifiers (your Apple/Google ID and email)
  - Your encrypted SQLite snapshot from our R2 storage
  - Per-install rate-limit metadata in our Worker's storage
  - Any encrypted file blobs in your Google Drive's `Remember4Me` folder
    (we instruct the app to delete these; you can also delete the folder
    yourself directly from drive.google.com)

  ## What we cannot delete (because we never had it)

  Because Remember4Me is end-to-end encrypted, we never possess the
  content of your notes, documents, tags, or summaries. We can confirm
  that the encrypted blobs are deleted, but there is no plaintext copy
  on our side to delete in the first place.

  ## Contact

  **Email:** renu.k.rjam.ai@gmail.com
