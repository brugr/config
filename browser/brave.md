# Brave

Brave doesn't let you import/export flags and settings, so these have to be done manually

## Settings `brave://settings`

Items marked in **bold** are more important to change, *imo*

First follow [Privacy Guides recommended settings](https://www.privacyguides.org/en/desktop-browsers/#brave), then continue below

* **Get Started** `brave://settings/getStarted`
  * Get started
    * On startup > Continue where you left off | *Personal preference*
  * New Tab Page
    * **Customize new tab page > Remove all the bloat/crypto shit**
* **Appearance** `brave://settings/appearance`
  * **Customize your toolbar > Remove all the bloat/crypto crap**
  * **Always show full URLs > Enabled**
  * Show rounded corners on main content areas > Disabled
* **Content** `brave://settings/braveContent`
  * Content
    * Show Wayback Machine prompt on 404 pages > Enabled
  * Containers
    * Enable Containers > Enabled | *Useful for different logins on the same site*
  * Speedreader
    * **Automatically use Speedreader when possible > Disabled** | *Can break some websites*
* **Shields** `brave://settings/shields`
  * Shields
    * **Block scripts > Disabled**
    * **Forget me when I close this site > Disabled**
    * Allow element blocking in private windows > Enabled
  * Social media blocking
    * Personal preference
* **Privacy and security** `brave://settings/privacy`
  * Privacy and security
    * **Security > Manage JavaScript optimization & security `brave://settings/content/v8` > Personal preference, usually enabled**
    * **WebRTC IP handling policy > Default public interface only,** *some websites break with Disable non-proxied UDP*
    * Local history retention > Forever | *Personal preference*
    * Block Microsoft Recall > Disabled | *Can break some screen-recording or VR overlay apps*
    * **Send a "Do Not Track" request with your browsing traffic > Leave Default, usually disabled** | *DNT headers don't do shit, some websites use it to fingerprint you more*
  * Tor windows
    * Only resolve .onion addresses in Tor windows > Enabled
  * **Data collection > Disable everything**
* **Web3** `brave://settings/web3`
  * Wallet
    * **Default *crypto* wallet > Extensions (no fallback)**
    * **Disable everything**
  * **Web3 Domains > Resolve *web3* domain names > Disabled**
* **Search engine** `brave://settings/search`
  * Improve search suggestions > Enabled | *Only recommended with a privacy respecting search engine or No Search trick below*
  * **Web Discovery Project > Disabled**
  * Manage search engines and site search
    * Site search > Add
      * Name: `No Search`
      * Shortcut: `nosearch`
      * URL: `https://%s`
    * Change shortcuts to primary search engine
    * Backout and set `No Search` as the default
    * Now use the shortcut in the address bar whenever you want to search something
* **Extensions** `brave://settings/extensions`
  * Media Router > Disabled | *Disables casting*
  * Widevine > Enabled | *Required by some streaming services*
* **Autofill and passwords** `brave://settings/autofill`
  * **Disable everything**

## Flags `brave://flags`

* V8 Jitless mode | `brave://flags/#brave-v8-jitless-mode` | Enabled  
*Will only be applied to websites that **aren't allowed** to use the V8 Javascript engine* `brave://settings/content/v8`
* Brave News prompt on New Tab Page | `brave://flags/#brave-news-peek` | **Disabled**
* Brave Tree Tab | `brave://flags/#brave-tree-tab` | Enabled  
*Also needs to be enabled inside **Settings > Tabs > Use vertical tabs > Use tree tabs***
* Brave AI Chat | `brave://flags/#brave-ai-chat` | **Disabled**
* Brave's AI browsing | `brave://flags/#brave-ai-chat-agent-profile` | **Disabled**
* Enable Email Aliases | `brave://flags/#brave-email-aliases` | **Disabled**
* Override download danger level | Enabled, **USE WITH CAUTION**, *Only matters if Safe Browsing is turned off*
