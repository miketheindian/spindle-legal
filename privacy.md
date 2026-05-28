 # Privacy Policy
                                                                                                                                                                                                                 
  **Effective: 2026-05-27**                                 

  Spindle is a vinyl-collection and listening tracker built by Mike                                                                                                                                              
  Warner. This policy describes what data Spindle collects, how it's
  used, and what control you have over it.                                                                                                                                                                       
                                                                                                                                                                                                                 
  Contact: **info@spindle.app**
  Moderation contact: **mod@spindle.app**                                                                                                                                                                        
                                                            
  ---

  ## 1. What we collect                                                                                                                                                                                          
   
  When you sign up and use Spindle, the following data is stored on                                                                                                                                              
  our servers (hosted by Supabase):                         
                                                                                                                                                                                                                 
  - **Account**: email address and a password hash. Used to sign you
    in and recover access.                                                                                                                                                                                       
  - **Profile**: username, display name, and optional bio. Visible to
    other signed-in Spindle users. If you've connected Discogs, your
    Discogs profile photo is loaded directly from Discogs and shown
    only to you — it is never uploaded to or stored on our servers.
  - **Your collection**: the records you've imported from Discogs                                                                                                                                                
    (album, artist, year, cover URL, format) plus any per-record
    customizations you've made in-app (vinyl color, design, etc.).                                                                                                                                               
  - **Listening history**: each spin you log — record, start time,                                                                                                                                               
    end time, optional side, optional mood, optional rating, optional                                                                                                                                            
    private notes.                                                                                                                                                                                               
  - **Social activity**: who you follow, your reactions, your                                                                                                                                                    
    comments on challenge picks, your optional captions on picks,                                                                                                                                                
    your optional public status note while spinning.
  - **Moderation activity**: reports you file and users you block.                                                                                                                                               
                                                                                                                                                                                                                 
  Spindle does **not** collect device contacts, location, photos,
  or any third-party tracking identifiers.                                                                                                                                                                                          
   
  ## 2. Third-party services                                                                                                                                                                                     
                                                            
  - **Supabase** hosts our database, authentication, and realtime                                                                                                                                                
    messaging. Data lives in Supabase's US-region servers under our
    account. See Supabase's privacy policy at https://supabase.com/privacy.                                                                                                                                      
  - **Discogs** is connected via OAuth when you import your 
    collection. Discogs tokens are stored only on the device that                                                                                                                                                
    authorized them — they're never synced to our servers.  
  - **PostHog** is our product analytics provider. We send a small
    set of typed product events (taps, screen transitions, completed
    spins) associated with your Spindle account ID so we can
    understand how Spindle is used and where it can improve. No
    email, display name, handle, search text, caption text, or other
    personal content is sent. See PostHog's privacy policy at
    https://posthog.com/privacy.
  - **Sentry** is our crash and error reporting provider. When the
    app crashes or hits an unexpected error, we send a diagnostic
    report (stack trace, app version, device model, OS version, and
    your Spindle account ID). Sensitive values like tokens, note
    text, and search queries are scrubbed client-side before sending.
    See Sentry's privacy policy at https://sentry.io/privacy.
  - **Last.fm** is optionally connected via OAuth so the app can
    scrobble completed spins to your Last.fm account. Last.fm
    receives the artist, album, and track title of each scrobbled
    spin plus the Last.fm username you authorized it with. Last.fm
    is not contacted unless you explicitly connect your account. See
    Last.fm's privacy policy at https://www.last.fm/legal/privacy.
                                                                                                                                                                                                                 
  We don't sell your data, don't share it with advertisers, and don't                                                                                                                                            
  use it for any purpose other than running Spindle.                                                                                                                                                             
                                                                                                                                                                                                                 
  ## 3. How we use it                                       

  - To show you your collection, history, stats, and challenges.                                                                                                                                                 
  - To show your public profile, picks, comments, status, and
    current spin to other Spindle users.                                                                                                                                                                         
  - To deliver realtime emoji reactions and presence to active spin
    rooms (these messages are **ephemeral** — never written to the                                                                                                                                               
    database).                                                                                                                                                                                                   
  - To send you notifications you've opted into (forgotten-spin                                                                                                                                                  
    reminders, streaks, challenge announcements).                                                                                                                                                                
  - To enforce community standards via the moderation system                                                                                                                                                     
    described in §6.                                                                                                                                                                                             
                                                                                                                                                                                                                 
  ## 4. Data retention and deletion                                                                                                                                                                              
   
  You can permanently delete your account from **Profile → Delete                                                                                                                                                
  Account** in the app. Deletion is immediate and cascades through
  the database — your records, spins, profile, comments, follows,                                                                                                                                                
  likes, and any captions or status notes are removed atomically.                                                                                                                                                
                                                                                                                                                                                                                 
  You can hide individual records from your collection                                                                                                                                                           
  (**Album detail → Remove from Spindle**) without deleting your                                                                                                                                                 
  account; hidden records are still accessible from                                                                                                                                                              
  **Profile → Hidden Records** so you can restore them.
                                                                                                                                                                                                                 
  ## 5. Children's privacy                                  
                                                                                                                                                                                                                 
  Spindle isn't directed at children under 13 and we don't knowingly                                                                                                                                             
  collect data from them. If you believe a child has signed up, email
  **mike@spindle.app** and we'll remove the account.                                                                                                                                                             
                                                            
  ## 6. User-generated content and moderation                                                                                                                                                                    
   
  Spindle includes user-generated text in the following surfaces:                                                                                                                                                
                                                            
  - Profile bio, display name, and username                                                                                                                                                                      
  - Captions you can attach to a challenge pick
  - Comments on other people's challenge picks                                                                                                                                                                   
  - A public status note shown while you're spinning                                                                                                                                                             
   
  We moderate these surfaces with a layered system:                                                                                                                                                              
                                                            
  ### 6.1 Report                                                                                                                                                                                                 
                                                            
  Every UGC surface has a **Report** action accessible via long-press                                                                                                                                            
  (picks, status notes) or a kebab/⋮ menu (profiles, comments).
  Reports are submitted to our `content_reports` table and tagged                                                                                                                                                
  with a reason: Spam, Harassment or hate, Sexually explicit / NSFW,
  Self-harm or dangerous, Illegal content, or Other.                                                                                                                                                             
                                                            
  **Operator review target: within 24 hours** of the report being                                                                                                                                                
  filed. Reports are triaged manually by Mike Warner. To follow up
  on a report or contest a moderation decision, email                                                                                                                                                            
  **mod@spindle.app**.                                                                                                                                                                                           
                                                                                                                                                                                                                 
  ### 6.2 Auto-suppression                                                                                                                                                                                       
                                                            
  When three distinct users have reported the same piece of content,
  that content is automatically hidden from everyone except the
  author. The author still sees their own content (the "shadow-ban"                                                                                                                                              
  property), but no one else does. An operator reviews the reports
  within 24 hours and either:                                                                                                                                                                                    
                                                                                                                                                                                                                 
  - Leaves the suppression in place if the reports are valid, or                                                                                                                                                 
  - Restores the content if the reports are invalid or coordinated.                                                                                                                                              
                                                            
  ### 6.3 Per-user shadow-ban                                                                                                                                                                                    
   
  When a user has accumulated **three suppressed pieces of content**,                                                                                                                                            
  their entire UGC footprint — captions, comments, profile fields,
  status notes — is hidden from every other user. The user                                                                                                                                                       
  themselves continues to see their own content. They receive no
  notification. This protects the community from repeat offenders                                                                                                                                                
  while avoiding adversarial escalation.                    
                                                                                                                                                                                                                 
  ### 6.4 Block                                             
                                                                                                                                                                                                                 
  Any user can block any other user via the kebab menu on a profile
  or a long-press on a pick row. Blocking is one-way and silent: the
  blocked user is not notified. After blocking:                                                                                                                                                                  
   
  - The blocked user's picks, comments, reactions, presence pings,                                                                                                                                               
    and live-spin status no longer appear anywhere in your view of
    Spindle.                                                                                                                                                                                                     
  - Your content remains visible to the blocked user (consistent                                                                                                                                                 
    with industry norms — blocks aren't broadcasts).
                                                                                                                                                                                                                 
  You can review and undo blocks at any time.               
                                                                                                                                                                                                                 
  ### 6.5 Rate limiting and anti-abuse                      

  - Each user can file at most **10 reports per 24-hour window**.                                                                                                                                                
  - Self-reports are blocked at the database level.
  - Duplicate reports on the same content are silently de-duplicated.                                                                                                                                            
  - All report and block actions are server-mediated via RPCs; the
    underlying tables refuse direct writes from clients.                                                                                                                                                         
                                                                                                                                                                                                                 
  ## 7. Your rights                                                                                                                                                                                              
                                                                                                                                                                                                                 
  - **Access**: every piece of data Spindle stores about you is
    visible to you in-app. We don't keep hidden profiles or shadow
    data.                                                                                                                                                                                                        
  - **Correction**: you can edit your profile, comments, status
    notes, and pick captions at any time.                                                                                                                                                                        
  - **Deletion**: as described in §4.                       
  - **Export**: a CSV export of your spin history is on our roadmap;                                                                                                                                             
    email **mike@spindle.app** in the meantime if you need a copy                                                                                                                                                
    before the in-app feature ships.                                                                                                                                                                             
                                                                                                                                                                                                                 
  ## 8. Security                                                                                                                                                                                                 
                                                            
  - All network traffic uses TLS.                                                                                                                                                                                
  - Authentication tokens are stored in platform secure storage
    (iOS Keychain, Android EncryptedSharedPreferences).                                                                                                                                                          
  - Our Discogs and Last.fm OAuth consumer secrets are stored only                                                                                                                                               
    on our server — never bundled into the app binary or transmitted
    to your device.                                                                                                                                                                                              
                                                            
  ## 9. Changes to this policy                                                                                                                                                                                   
                                                            
  We'll update the **Effective** date at the top of this document                                                                                                                                                
  when the policy materially changes. Significant changes will be
  announced via in-app banner before they take effect.                                                                                                                                                           
                                                                                                                                                                                                                 
  ## 10. Contact
                                                                                                                                                                                                                 
  - General: **info@spindle.app**                                                                                                                                                                                
  - Moderation: **mod@spindle.app**
