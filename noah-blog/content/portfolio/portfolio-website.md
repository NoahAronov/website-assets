
# <!-- STEP ONE -->  
<h1 style="text-align:center">Portfolio Website with WAF and CI/CD</h1>
<br>

---

*This project is a security portfolio website using a registered domain, custom DNS, a basic CI/CD pipeline, a static site generator, serverless functions, email routing, a developer environment, global CDN, load balancing, and numerous speed optimizations.*

*Incorporates security features like multi factor authentication, passkeys, TLS encryption, SSL certificates, DDoS mitigation, web application firewall (WAF), CAPTCHA challenge, bot and AI security, email anti-phishing mitigation, role-based account control, 3-2-1 backups, and worldwide server failover.*

*Uses Porkbun, Cloudflare, and GitHub services. Uses Hugo, Anatole, terminalCV, and Lynx for static site generation. Uses HTML, CSS, Markdown, TOML, and YAML languages.*

---

<h2 style="text-align:center">Contents:</h2>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <ol>
    <li><a href="#1">Registered a custom domain with Porkbun.</a></li>
    <li><a href="#2">Secured Porkbun account with a passkey in Bitwarden password manager.</a></li>
    <li><a href="#3">Registered a developer account with Cloudflare.</a></li>
    <li><a href="#4">Secured Cloudflare account with a passkey in Bitwarden.</a></li>
    <li><a href="#5">Set DNS nameservers to Cloudflare in Porkbun domain management.</a></li>
    <li><a href="#6">Configured email routing with custom domain in Cloudflare.</a></li>
    <li><a href="#7">Configured core security and speed settings in Cloudflare.</a></li>
    <li><a href="#8">Set TLS encryption mode to "Full (strict)" in Cloudflare.</a></li>
    <li><a href="#9">Reviewed security settings along the traffic sequence as it proxies through Cloudflare.</a></li>
    <li><a href="#10">Set up a developer environment for the project.</a></li>
    <li><a href="#11">Installed Hugo and dependencies.</a></li>
    <li><a href="#12">Initialized Hugo website, installed theme as a git submodule.</a></li>
    <li><a href="#13">Customized and added content to website.</a></li>
    <li><a href="#14">Created a repository for the project in GitHub.</a></li>
    <li><a href="#15">Secured GitHub account with a passkey in Bitwarden.</a></li>
    <li><a href="#16">Integrated GitHub repository with Cloudflare Pages static web hosting.</a></li>
    <li><a href="#17">Created Cloudflare Worker serverless function to push website from GitHub repository to Cloudflare Pages.</a></li>
    <li><a href="#18">Set custom DNS records for Cloudflare Pages website in Cloudflare.</a></li>
    <li><a href="#19">Ran a speed test in Cloudflare Observatory.</a></li>
  </ol>
</div>
<br>

<!-- STEP ONE --> 
<h2 id="1" style="text-align:center">1. Registered a custom domain with Porkbun.</h2>
<p style="text-align:center"><a href="https://porkbun.com/">Porkbun.com</a></p>
<div style="text-align:center">
  <img src="/images/portfolio/port4.png" alt="Porkbun tools">
  <p><i>Porkbun tools</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port5.png" alt="Porkbun features">
  <p><i>Porkbun features</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port1.png" alt="Porkbun domain">
  <p><i>Porkbun domain management</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Porkbun security features:</b></p>
  <ul style="margin-top:0">
    <li>Free WHOIS Privacy</li>
    <li>Free SSL Certificates issued by <a href="https://letsencrypt.org/">Let's Encrypt</a></li>
    <li>Cloudflare DNS Management</li>
  </ul>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p>
  <a href="https://www.cloudflare.com/learning/dns/glossary/what-is-a-domain-name/">What is a domain name?</a><br>
  <a href="https://porkbun.com/products/whois_privacy">What is WHOIS privacy?</a><br>
  <a href="https://letsencrypt.org/how-it-works/">What is an SSL certificate?</a><br>
  <a href="https://www.cloudflare.com/learning/dns/what-is-dns/">What is DNS?</a><br>
  </p>
</div>
<br>


<!-- STEP TWO -->
<h2 id="2" style="text-align:center">2. Secured Porkbun account with a passkey in Bitwarden password manager.</h2>
<p style="text-align:center"><a href="https://bitwarden.com/">Bitwarden.com</a></p>
<div style="text-align:center">
  <img src="/images/portfolio/port7.png" alt="Bitwarden diagram">
  <p><i>Bitwarden diagram</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port2.png" alt="Porkbun passkey">
  <p><i>Passkey in Porkbun</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port3.png" alt="Passkey in Bitwarden">
  <p><i>Passkey in Bitwarden</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Bitwarden security features:</b></p>
  <ul style="margin-top:0">
    <li>Open source with regular third party audits</li>
    <li>Zero-knowledge end-to-end AES-256 bit encryption, salted hashing, and PBKDF2 SHA-256 authentication process</li>
    <li>Compliant with GDPR, SOC 2, HIPAA, Privacy Shield, and CCPA standards</li>
    <li>Passkey storage and management</li>
    <li>Email alias integration</li>
    <li>Data breach reports</li>
  </ul>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p>
  <a href="https://bitwarden.com/passwordless-passkeys/">What is a passkey?</a><br>
  <a href="https://bitwarden.com/products/">What is a password manager?</a><br>
  <a href="https://simplelogin.io/">What is an email alias?</a><br>
  </p>
</div>
<br>


<!-- STEP THREE -->
<h2 id="3" style="text-align:center">3. Registered a developer account with Cloudflare.</h2>
<p style="text-align:center"><a href="https://www.cloudflare.com/developer-platform/">Cloudflare.com</a></p>
<div style="text-align:center">
  <img src="/images/portfolio/port8.png" alt="Cloudflare Developer Platform">
  <p><i>Cloudflare Developer Platform</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port11.png" alt="Platform benefits">
  <p><i>Platform benefits</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port9.png" alt="Platform features">
  <p><i>Platform features</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port10.png" alt="Platform tools">
  <p><i></i>Platform tools</p>
</div>
<br>


<!-- STEP FOUR -->
<h2 id="4" style="text-align:center">4. Secured Cloudflare account with a passkey in Bitwarden.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port12.png" alt="Passkey in Cloudflare">
  <p><i>Passkey in Cloudflare</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port13.png" alt="Passkey in Bitwarden">
  <p><i>Passkey in Bitwarden</i></p>
</div>
<br>


<!-- STEP FIVE -->
<h2 id="5" style="text-align:center">5. Set DNS nameservers to Cloudflare in Porkbun domain management.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port14.png" alt="Porkbun authoritative nameservers">
  <p><i>Porkbun authoritative nameservers</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port17.png" alt="Cloudflare DNS">
  <p><i>Cloudflare DNS</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port18.png" alt="Cloudflare DNS protection">
  <p><i>Cloudflare DNS protection</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Cloudflare DNS security features:</b></p>
  <ul style="margin-top:0">
    <li>Unlimited and unmetered DDoS mitigation</li>
    <li>Protection from route leaks and hijacking</li>
    <li>Load balancing</li>
    <li>Support for DNSSEC</li>
    <li>Support for DNS over TLS (DoT)</li>
    <li>CDN: redundancy across 320 cities</li>
    <li>Email security DNS records: SPF, DKIM, DMARC</li>
    <li>Advanced real-time DNS analytics</li>
    <li>Cloudflare Universal SSL certificate</li>
    <li>Cloudflare TLS encryption modes</li>
    <li>Role-based account control</li>
    <li>Simple bot mitigation</li>
  </ul>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p>
  <a href="https://www.cloudflare.com/learning/ddos/what-is-a-ddos-attack/">What is DDoS?</a><br>
  <a href="https://www.cloudflare.com/learning/security/glossary/bgp-hijacking/">What is BGP hijacking?</a><br>
  <a href="https://www.cloudflare.com/learning/dns/dns-security/">What is DNSSEC?</a><br>
  <a href="https://www.cloudflare.com/learning/dns/dns-over-tls/">What is DoT?</a><br>
  <a href="https://www.cloudflare.com/learning/cdn/what-is-a-cdn/">What is CDN?</a><br>
  <a href="https://www.cloudflare.com/learning/dns/dns-records/dns-spf-record/">What is SPF?</a><br>
  <a href="https://www.cloudflare.com/learning/dns/dns-records/dns-dkim-record/">What is DKIM?</a><br>
  <a href="https://www.cloudflare.com/learning/dns/dns-records/dns-dmarc-record/">What is DMARC?</a><br>
  <a href="https://www.cloudflare.com/learning/ssl/transport-layer-security-tls/">What is TLS?</a><br>
  </p>
</div>
<br>


<!-- STEP SIX -->
<h2 id="6" style="text-align:center">6. Configured email routing with custom domain in Cloudflare.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port15.png" alt="Cloudflare Email Routing">
  <p><i>Cloudflare Email Routing</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port16.png" alt="Email Routing set">
  <p><i>Email Routing set</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Cloudflare Email Routing security features:</b></p>
  <ul style="margin-top:0">
    <li>Email contents are not stored or accessed by Cloudflare</li>
    <li>Anti-spam and phishing detection</li>
    <li>Advanced real-time email analytics</li>
    <li>Process emails with logic using Cloudflare Workers</li>
    <li>Primary email address is not shared</li>
  </ul>
</div>
<br>


<!-- STEP SEVEN -->
<h2 id="7" style="text-align:center">7. Configured core security and speed settings in Cloudflare.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port19.png" alt="Core security and speed settings">
  <p><i>Core security and speed settings</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Cloudflare core security and speed features:</b></p>
  <ul style="margin-top:0">
    <li><a href="https://developers.cloudflare.com/speed/optimization/protocol/http2-to-origin/">HTTP/2 to Origin</a>: Allow HTTP/2 requests between Cloudflare's edge and your origin to improve performance.</li>
    <li><a href="https://developers.cloudflare.com/speed/optimization/protocol/http3/">HTTP/3 (with QUIC)</a>: Accelerate page loads by enabling visitors’ browsers and web servers to communicate as efficiently as possible.</li>
    <li><a href="https://developers.cloudflare.com/speed/optimization/protocol/0-rtt-connection-resumption/">0-RTT Connection Resumption</a>: Improves site performance for previous site visitors.<br>
    This most benefits end users who visit an application regularly or who use mobile networks.</li>
    <li><a href="https://developers.cloudflare.com/ssl/edge-certificates/additional-options/always-use-https/">Always Use HTTPS</a>: Increase security by redirecting all your visitor requests from http to https.</li>
    <li><a href="https://developers.cloudflare.com/ssl/edge-certificates/additional-options/tls-13/">TLS 1.3</a>: Secures communications and improves page load times.</li>
    <li><a href="https://developers.cloudflare.com/rules/normalization/">Normalize incoming URLs</a>: Modifies the URLs of incoming requests so that they conform to a consistent formatting standard.</li>
    <li><a href="https://developers.cloudflare.com/network/websockets/">WebSockets</a>: Protect WebSocket connections which increase connection speeds by enabling the client<br>
    and the origin to pass data back and forth without having to reestablish sessions. </li>
    <li><a href="https://developers.cloudflare.com/network/onion-routing/">Onion Routing</a>: Increases security by ensuring Tor network users can no longer access sites via exit nodes which can be<br>
    compromised and helps only serve challenges to malicious bot traffic.</li>
    <li><a href="https://developers.cloudflare.com/waf/tools/browser-integrity-check/">Browser Integrity Check</a>: Increases security by looking for common HTTP headers abused most commonly by spammers and denies access to your page.<br>
    It also challenges visitors without a user agent or with a non-standard user agent such as commonly used by abusive bots, crawlers, or visitors.</li>
    <li><a href="https://developers.cloudflare.com/waf/tools/scrape-shield/hotlink-protection/">Hotlink Protection</a>: Prevents your images from being used by other sites, which can reduce the bandwidth consumed by your origin server.</li>
  </ul>
</div>
<br>


<!-- STEP EIGHT -->
<h2 id="8" style="text-align:center">8. Set TLS encryption mode to "Full (strict)" in Cloudflare.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port20.png" alt="SSL/TLS encryption mode">
  <p><i>SSL/TLS encryption mode</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Cloudflare SSL/TLS security features:</b></p>
  <ul style="margin-top:0">
    <li>Enable encryption end-to-end and enforce validation on origin certificates</li>
    <li>Use Cloudflare’s Origin CA to generate certificates for your origin</li>
    <li>SSL/TLS Recommender runs a periodic origin scan and sends you an email if a more secure option is possible</li>
    <li>Customize different aspects of your edge certificates, from enabling Opportunistic Encryption to specifying a Minimum TLS Version</li>
    <li>Authenticated origin pull: Ensure all requests to your origin server originate from the Cloudflare network</li>
    <li>Set up alerts related to certificate validation status, issuance, deployment, renewal, and expiration</li>
  </ul>
</div>
<br>


<!-- STEP NINE -->
<h2 id="9" style="text-align:center">9. Reviewed security settings along the traffic sequence as it proxies through Cloudflare.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port21.png" alt="Traffic sequence">
  <p><i>Traffic sequence</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port22.png" alt="Cloudflare DDoS mitigation">
  <p><i>Cloudflare DDoS mitigation</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port23.png" alt="Traffic sequence with mitigation">
  <p><i>Traffic sequence with mitigation</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port24.png" alt="Bots security">
  <p><i>Bots security</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port25.png" alt="Cloudflare WAF">
  <p><i>Cloudflare WAF</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Cloudflare DDoS security features:</b></p>
  <ul style="margin-top:0">
    <li>Automatic DDoS protection that constantly analyzes traffic and generates real-time<br>
    signatures to mitigate attacks across the network and application layers</li>
    <li>Cloudflare’s autonomous DDoS protection systems use a set of dynamic rules that<br>
    scan for attack patterns, known attack tools, suspicious patterns, protocol violations,<br>
    requests causing large amounts of origin errors, excessive traffic hitting the<br> 
    origin/cache, and additional attack vectors.</li>
    <li>HTTP DDoS attack protection: Ruleset managed by Cloudflare that automatically<br> 
    mitigates HTTP-based DDoS attacks such as HTTP floods, amplification<br> 
    HTTP attacks, and reflection HTTP attacks.</li>
    <li>SSL/TLS DDoS attack protection: Automatic mitigation of SSL/TLS based DDoS<br> 
    attacks and encryption-based attacks such as DDoS attacks, SSL exhaustion floods,<br> 
    and SSL negotiation attacks.</li>
    <li>Network-layer DDoS attack protection: Automatic mitigation of network-layer<br> 
    DDoS attacks such as ACK floods, SYN-ACK amplification attacks, UDP attacks,<br> 
    ICMP attacks and DDoS attacks launched by botnets such as Mirai.</li>
  </ul>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Cloudflare Rules features:</b></p>
  <ul style="margin-top:0">
    <li>Transform Rules: Adjust the URI path, query string, and HTTP headers of<br> 
    requests and responses at the edge. Transformed traffic is then used as<br> 
    input for other Cloudflare products.</li>
    <li>Page Rules: Trigger certain actions whenever a request matches a defined URL pattern.</li>
    <li>Origin Rules: Customize where matching traffic will go and with which parameters.<br> 
    Allows host header, SNI, DNS record, and destination port overrides.</li>
    <li>Cache Rules: Specify which resources should be cached and for how long.</li>
    <li>Configuration Rules: Customize configuration settings for matching incoming requests.</li>
    <li>Redirect Rules: Create rules to redirect visitors from a source URL to a target URL.</li>
    <li>IP Access Rules: Can be based on IP address, IP address range, Autonomous<br> 
    System Number (ASN) or country.</li>
  </ul>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Cloudflare Bots security features:</b></p>
  <ul style="margin-top:0">
    <li>Bot Fight Mode: Challenge requests that match patterns of known bots, before<br> 
    they access your site. This feature includes JavaScript Detections.</li>
    <li>Block AI Scrapers and Crawlers: Block bots from scraping your content for<br> 
    AI applications like model training.</li>
  </ul>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Cloudflare WAF security features:</b></p>
  <ul style="margin-top:0">
    <li>The Cloudflare WAF runs on the Cloudflare global network and sits in front<br>
    of web applications to stop a wide range of real-time attacks using powerful rulesets,<br> 
    advanced rate limiting, exposed credential checks, uploaded content scanning,<br> 
    and other security measures.</li>
    <li>Managed ruleset providing mitigation against high profile vulnerabilities. </li>
    <li>mTLS-enforced authentication: Block requests from devices without a<br> 
    valid known client SSL/TLS certificate.</li>
    <li>Zone lockdown: Allow only specific IP addresses to access certain URLs<br> 
    such as an admin or protected area on your website.</li>
  </ul>
</div>
<br>


<!-- STEP TEN -->
<h2 id="10" style="text-align:center">10. Set up a developer environment for the project.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port26.png" alt="Developer environment">
  <p><i>Developer environment</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p style="margin-bottom:0"><b>Components:</b></p>
  <ul style="margin-top:0">
    <li><a href="https://en.wikipedia.org/wiki/Windows_10">Windows 10</a>: host operating system</li>
    <li><a href="https://learn.microsoft.com/en-us/windows/wsl/about">WSL2</a>: runs linux kernel in Windows</li>
    <li><a href="https://www.debian.org/">Debian 12</a>: linux operating system in WSL2</li>
    <li><a href="https://floorp.app/">Floorp</a>: security focused browser based on Firefox</li>
    <li><a href="https://obsidian.md/">Obsidian</a>: note taking app using markdown</li>
    <li><a href="https://github.com/apps/desktop">GitHub Desktop</a>: GitHub GUI client</li>
    <li><a href="https://www.sublimetext.com/">Sublime</a>: text editor</li>
    <li><a href="https://code.visualstudio.com/">VS Code</a>: integrated developer environment</li>
    <li><a href="https://tabby.sh/">Tabby</a>: SSH and local terminal with secrets management</li>
    <li><a href="https://www.zsh.org/">zsh</a>: interactive command shell</li>
    <li><a href="https://starship.rs/">Starship</a>: blazing fast prompt for any shell</li>
    <li><a href="https://phoenixnap.com/kb/nala-apt">nala</a>: frontend for APT package manager</li>
    <li><a href="https://packages.debian.org/git">git</a>: git CLI client</li>
    <li><a href="https://cli.github.com/">gh</a>: github CLI client</li>
  </ul>
</div>
<br>


<!-- STEP ELEVEN -->
<h2 id="11" style="text-align:center">11. Installed Hugo and dependencies.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port27.png" alt="Installing Hugo">
  <p><i>Installing Hugo</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p>
  <a href="https://www.cloudflare.com/learning/performance/static-site-generator/">What is a static site generator?</a><br>
  </p>
</div>
<br>


<!-- STEP TWELVE -->
<h2 id="12" style="text-align:center">12. Initialized Hugo website, installed theme as a git submodule.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port28.png" alt="Initialized Hugo website">
  <p><i>Initialized Hugo website</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port29.png" alt="Installed theme as submodule">
  <p><i>Installed theme as submodule</i></p>
</div>
<br>


<!-- STEP THIRTEEN -->
<h2 id="13" style="text-align:center">13. Customized and added content to website.</h2>
<br>


<!-- STEP FOURTEEN -->
<h2 id="14" style="text-align:center">14. Created a repository for the project in GitHub.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port30.png" alt="Website repositories">
  <p><i>Website repositories</i></p>
</div>
<br>


<!-- STEP FIFTEEN -->
<h2 id="15" style="text-align:center">15. Secured GitHub account with a passkey in Bitwarden.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port31.png" alt="Passkey in GitHub">
  <p><i>Passkey in GitHub</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port32.png" alt="Passkey in Bitwarden">
  <p><i>Passkey in Bitwarden</i></p>
</div>
<br>


<!-- STEP SIXTEEN -->
<h2 id="16" style="text-align:center">16. Integrated GitHub repository with Cloudflare Pages static web hosting.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port33.png" alt="Cloudflare Pages in GitHub">
  <p><i>Cloudflare Pages in GitHub</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port34.png" alt="Cloudflare Pages">
  <p><i>Cloudflare Pages</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port35.png" alt="Cloudflare Pages features">
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port36.png" alt="Cloudflare Pages features">
  <p><i>Cloudflare Pages features</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p>
  <a href="https://developers.cloudflare.com/pages/framework-guides/deploy-anything/">What is a static web page?</a><br>
  <a href="https://www.cloudflare.com/developer-platform/pages/">What is Cloudflare Pages?</a><br>
  </p>
</div>
<br>


<!-- STEP SEVENTEEN -->
<h2 id="17" style="text-align:center">17. Created Cloudflare Worker serverless function to push website from GitHub repository to Cloudflare Pages.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port37.png" alt="Cloudflare Workers with automatic build">
  <p><i>Cloudflare Workers with automatic build</i></p>
</div>
<br>
<div style="text-align:center">
  <img src="/images/portfolio/port38.png" alt="Cloudflare Workers features">
  <p><i>Cloudflare Workers features</i></p>
</div>
<br>
<div style="text-align:left;display:flex;flex-direction:column;align-items:center;">
  <p>
  <a href="https://www.cloudflare.com/learning/serverless/what-is-serverless/">What is a serverless function?</a><br>
  <a href="https://www.cloudflare.com/developer-platform/workers/pages">What is Cloudflare Workers?</a><br>
  </p>
</div>
<br>


<!-- STEP EIGHTEEN -->
<h2 id="18" style="text-align:center">18. Set custom DNS records for Cloudflare Pages website in Cloudflare.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port39.png" alt="Cloudflare Pages custom domain">
  <p><i>Cloudflare Pages custom domain</i></p>
</div>
<br>


<!-- STEP NINETEEN -->
<h2 id="19" style="text-align:center">19. Ran a speed test in Cloudflare Observatory.</h2>
<div style="text-align:center">
  <img src="/images/portfolio/port40.png" alt="Cloudflare Observatory speed test">
  <p><i>Cloudflare Observatory speed test</i></p>
</div>
<br>


<h2 style="text-align:center"></h2>


