# Aetherinox CSF Firewall Fork - Change Documentation

This document tracks all changes between the official CSF Firewall v15.00 (GPLv3) and the Aetherinox fork.

## Summary

| Category          | Count |
| ----------------- | ----- |
| Modified files    | 164   |
| New files         | 31    |
| Files removed     | 0     |
| Total differences | 195   |

**Fork Repository:** <https://github.com/Aetherinox/csf-firewall>

**Official CSF Repository:** <https://github.com/centminmod/configserver-scripts>

---

## Repository State (as of 2025-12-18)

| Repository      | HEAD Commit   | Date       | Message                                                                   |
| --------------- | ------------- | ---------- | ------------------------------------------------------------------------- |
| Official CSF    | `d04e808`     | 2025-09-04 | add CSF community sentiment, discussions and alternative discussion research |
| Aetherinox Fork | `ae9c78a6f`   | 2025-12-18 | docs(mkdocs): update changelog                                            |

---

## Change Statistics

| Metric            | Value      |
| ----------------- | ---------- |
| Lines added       | 58,556     |
| Lines removed     | 26,788     |
| Net change        | +31,768    |
| Fork size         | 13,108 KB  |
| Official size     | 2,910 KB   |
| Size difference   | +10,198 KB |

### Most Changed Files (by commit count)

| Rank | File                              | Commits |
| ---- | --------------------------------- | ------- |
| 1    | `ConfigServer/Config.pm`          | 9       |
| 2    | `ConfigServer/ServerCheck.pm`     | 9       |
| 3    | `ConfigServer/RBLCheck.pm`        | 8       |
| 4    | `ConfigServer/DisplayUI.pm`       | 7       |
| 5    | `ConfigServer/DisplayResellerUI.pm` | 6     |
| 6    | `ConfigServer/AbuseIP.pm`         | 5       |
| 7    | `ConfigServer/CheckIP.pm`         | 5       |
| 8    | `ConfigServer/CloudFlare.pm`      | 5       |
| 9    | `ConfigServer/RegexMain.pm`       | 5       |
| 10   | `ConfigServer/GetEthDev.pm`       | 4       |

---

## New Files (31 files)

Files that exist only in the Aetherinox fork.

### Branding Assets

| File                                                             | Description              | Initial Commit                                                   |
| ---------------------------------------------------------------- | ------------------------ | ---------------------------------------------------------------- |
| `csf-firewall-aetherinox/src/csf/csf-logo.svg`                   | Main CSF logo (SVG)      | `9b1711ac1` docs(img): update csf logos                          |
| `csf-firewall-aetherinox/src/csf/csf-logo-alt.svg`               | Alternate CSF logo (SVG) | `9b1711ac1` docs(img): update csf logos                          |
| `csf-firewall-aetherinox/src/csf/csf.png`                        | CSF logo (PNG)           | `62743b25d` chore: daily cleanup                                 |
| `csf-firewall-aetherinox/src/da/images/csf-logo.svg`             | DirectAdmin logo         | `9b1711ac1` docs(img): update csf logos                          |
| `csf-firewall-aetherinox/src/da/images/csf-logo-alt.svg`         | DirectAdmin alt logo     | `9b1711ac1` docs(img): update csf logos                          |
| `csf-firewall-aetherinox/src/da/images/csf.png`                  | DirectAdmin logo PNG     | `62743b25d` chore: daily cleanup                                 |
| `csf-firewall-aetherinox/src/interworx/images/csf-logo.svg`      | InterWorx logo           | `9b1711ac1` docs(img): update csf logos                          |
| `csf-firewall-aetherinox/src/interworx/images/csf-logo-alt.svg`  | InterWorx alt logo       | `9b1711ac1` docs(img): update csf logos                          |
| `csf-firewall-aetherinox/src/interworx/images/csf.png`           | InterWorx logo PNG       | `62743b25d` chore: daily cleanup                                 |
| `csf-firewall-aetherinox/src/ui/images/csf-logo.svg`             | Generic UI logo          | `9b1711ac1` docs(img): update csf logos                          |
| `csf-firewall-aetherinox/src/ui/images/csf-logo-alt.svg`         | Generic UI alt logo      | `9b1711ac1` docs(img): update csf logos                          |
| `csf-firewall-aetherinox/src/ui/images/csf.png`                  | Generic UI logo PNG      | `62743b25d` chore: daily cleanup                                 |
| `csf-firewall-aetherinox/src/webmin/csf/images/csf-logo.svg`     | Webmin logo              | `716cd916e` chore: remove excess images, migrate to name scheme  |
| `csf-firewall-aetherinox/src/webmin/csf/images/csf-logo-alt.svg` | Webmin alt logo          | `716cd916e` chore: remove excess images, migrate to name scheme  |
| `csf-firewall-aetherinox/src/webmin/csf/images/csf.png`          | Webmin logo PNG          | `62743b25d` chore: daily cleanup                                 |

### JavaScript Assets

| File                                                             | Description         | Initial Commit                                               |
| ---------------------------------------------------------------- | ------------------- | ------------------------------------------------------------ |
| `csf-firewall-aetherinox/src/csf/csf.min.js`                     | Minified CSF JS     | `4f3d228e3` feat: add new theme selector; dark & light theme |
| `csf-firewall-aetherinox/src/csf/csfont.min.js`                  | Font JavaScript     | `718dddcfa` Sync 12/01/2025                                  |
| `csf-firewall-aetherinox/src/da/images/csf.min.js`               | DirectAdmin JS      | `4f3d228e3` feat: add new theme selector; dark & light theme |
| `csf-firewall-aetherinox/src/da/images/csfont.min.js`            | DirectAdmin font JS | `718dddcfa` Sync 12/01/2025                                  |
| `csf-firewall-aetherinox/src/interworx/images/csf.min.js`        | InterWorx JS        | `4f3d228e3` feat: add new theme selector; dark & light theme |
| `csf-firewall-aetherinox/src/interworx/images/csfont.min.js`     | InterWorx font JS   | `718dddcfa` Sync 12/01/2025                                  |
| `csf-firewall-aetherinox/src/ui/images/csf.min.js`               | Generic UI JS       | `4f3d228e3` feat: add new theme selector; dark & light theme |
| `csf-firewall-aetherinox/src/ui/images/csfont.min.js`            | Generic UI font JS  | `718dddcfa` Sync 12/01/2025                                  |
| `csf-firewall-aetherinox/src/webmin/csf/images/csf.min.js`       | Webmin JS           | `4f3d228e3` feat: add new theme selector; dark & light theme |
| `csf-firewall-aetherinox/src/webmin/csf/images/csfont.min.js`    | Webmin font JS      | `718dddcfa` Sync 12/01/2025                                  |

### New Shell Scripts

| File                                     | Description               | Initial Commit                          |
| ---------------------------------------- | ------------------------- | --------------------------------------- |
| `csf-firewall-aetherinox/src/csfpre.sh`  | Pre-firewall hook script  | `62743b25d` chore: daily cleanup        |
| `csf-firewall-aetherinox/src/csfpost.sh` | Post-firewall hook script | `62743b25d` chore: daily cleanup        |
| `csf-firewall-aetherinox/src/global.sh`  | Global shell functions    | `25a7d5911` docs(man): update man pages |

### Configuration and SSL

| File                                                    | Description                | Initial Commit                                 |
| ------------------------------------------------------- | -------------------------- | ---------------------------------------------- |
| `csf-firewall-aetherinox/src/regex.txt`                 | Custom regex patterns      | `62743b25d` chore: daily cleanup               |
| `csf-firewall-aetherinox/src/ui/ssl-expired/server.crt` | Expired SSL cert (testing) | `5de621cd4` perf(ui): add preload optimization |
| `csf-firewall-aetherinox/src/ui/ssl-expired/server.key` | Expired SSL key (testing)  | `5de621cd4` perf(ui): add preload optimization |

---

## Modified Files - Core Scripts

### csf.pl (Main Firewall Script)

**Path:** `csf-firewall-aetherinox/src/csf.pl`

**Commit History (Recent):**

| Commit      | Description                                                                              |
| ----------- | ---------------------------------------------------------------------------------------- |
| `365e582f3` | fix(ui): incorrectly adding gap between first and second line in web interface           |
| `758e1180e` | fix(cli): detect tty for colored or clean output in responses                            |
| `c3c1127f7` | fix(cwp): sanitize and strip color codes for cwp version status                          |
| `ec339615a` | chore(csf): update log functionality output for users                                    |
| `cbc62a6d2` | style(csf): clean up command dictionary                                                  |
| `86ff22164` | feat(license): add new funcs for license and insiders checks                             |
| `05a25350f` | feat(cli): add command `--listports`, `-lp` #57                                          |
| `3ba60d17f` | feat(cli): add command `--removeport`, `-rp` #57                                         |
| `ac9e05a6a` | feat(cli): add command `--addport`, `-ap` #57                                            |
| `7f40ff7cd` | refactor(csf): update module output for updates                                          |
| `6a8d569b8` | feat(csf): add warning to console output when using default web ui username and password |

**Key Changes:**

- **New CLI Commands:** `--listports/-lp`, `--addport/-ap`, `--removeport/-rp` for port management (#57)
- **TTY Detection:** Colored output detection for cleaner CLI responses
- **License Functions:** New licensing and insiders check functionality
- **UI Fixes:** Web interface formatting improvements
- **Security Warning:** Console warning when using default web UI credentials

### lfd.pl (Login Failure Daemon)

**Path:** `csf-firewall-aetherinox/src/lfd.pl`

**Commit History:**

| Commit      | Description                                                                              |
| ----------- | ---------------------------------------------------------------------------------------- |
| `6a8d569b8` | feat(csf): add warning to console output when using default web ui username and password |

**Key Changes:**

- Security warning for default credentials

### csf.conf (Main Configuration)

**Path:** `csf-firewall-aetherinox/src/csf.conf`

**Commit History (Recent):**

| Commit      | Description                                                                               |
| ----------- | ----------------------------------------------------------------------------------------- |
| `f8f7f0d03` | feat(ui): add new setting `SPONSOR_HIDE_ICON` #72                                         |
| `9a1625b96` | style(generic): update formatting                                                         |
| `78a50b947` | chore: add input value type to LF_MODSEC_PERM comments #59                                |
| `a4a27599e` | chore: update config description for `LF_MODSEC` #59                                      |
| `ae27d1eb0` | feat: add insiders config items                                                           |
| `9a5cacfe0` | feat(ui): add highlighter classes "Firewall Configuration" page                           |
| `80dd350a2` | feat(ui): add two settings: `UI_LOGS_REFRESH_TIME` and `UI_LOGS_START_PAUSED` #25         |
| `fba868408` | refactor(conf): format comments for web interface                                         |
| `a07d9861b` | feat: add content-security-policy to web interface; new settings                          |
| `21338f61b` | feat: add login failure notification to login page; new setting `UI_RETRY_SHOW_REMAINING` |
| `aa1c52139` | chore(conf): update configs                                                               |
| `915bd564c` | feat: add new `csf.conf` setting `UI_BLOCK_PRIVATE_NET`                                   |
| `4b6cc3689` | feat: add env var `UI_LOGS_REFRESH`                                                       |
| `488e02495` | feat: add env var `UI_BLOCK_PRIVATE_NET`                                                  |

**New Configuration Options:**

| Setting                   | Description                   | Issue |
| ------------------------- | ----------------------------- | ----- |
| `SPONSOR_HIDE_ICON`       | Hide sponsor icon in UI       | #72   |
| `UI_LOGS_REFRESH_TIME`    | Log refresh interval          | #25   |
| `UI_LOGS_START_PAUSED`    | Start with logs paused        | #25   |
| `UI_RETRY_SHOW_REMAINING` | Show remaining login attempts | -     |
| `UI_BLOCK_PRIVATE_NET`    | Block private network ranges  | -     |
| `UI_LOGS_REFRESH`         | Log refresh toggle            | -     |

---

## Modified Files - ConfigServer Modules (24 files)

All Perl modules in `csf-firewall-aetherinox/src/ConfigServer/` directory.

### DisplayUI.pm (Web Interface)

**Commit History:**

| Commit      | Description                                                                                |
| ----------- | ------------------------------------------------------------------------------------------ |
| `365e582f3` | fix(ui): incorrectly adding gap between first and second line in web interface             |
| `69a1c24cf` | fix(webmin): add webmin `settings` button to interface without breaking theme js           |
| `4bd6de54b` | fix(webmin): ensure each setting is properly formatted, pre-wrap descriptions              |
| `f8f7f0d03` | feat(ui): add new setting `SPONSOR_HIDE_ICON` #72                                          |
| `2a061110e` | feat(ui): hide sponsor button if `SPONSOR_LICENSE` specified, or `UI_SPONSOR_HIDE = 1` #72 |
| `185654edc` | feat(ui): remove beating heart animation for sponsor icon #72                              |

**Key Changes:**

- Sponsor icon visibility controls
- Webmin settings button integration
- UI formatting fixes
- Setting description formatting

### DisplayResellerUI.pm

**Changes:** Reseller UI modifications paralleling DisplayUI.pm changes

### AbuseIP.pm

**Commit History:**

| Commit      | Description                                                                  |
| ----------- | ---------------------------------------------------------------------------- |
| `fb77803d9` | chore: update csf main repo for `v15.01` server changes                      |
| `ee9c4339a` | refactor: update headers, commenting in config files, line length conformity |

**Changes:** Header updates, code formatting

### Other Modified Modules

| Module           | Primary Changes               |
| ---------------- | ----------------------------- |
| `CheckIP.pm`     | Header updates, formatting    |
| `CloudFlare.pm`  | Header updates, formatting    |
| `Config.pm`      | Configuration parsing updates |
| `GetEthDev.pm`   | Network device detection      |
| `GetIPs.pm`      | IP retrieval improvements     |
| `KillSSH.pm`     | SSH rate limiting             |
| `Logger.pm`      | Logging enhancements          |
| `LookUpIP.pm`    | IP lookup functionality       |
| `Messenger.pm`   | Messaging updates             |
| `Ports.pm`       | Port management               |
| `RBLCheck.pm`    | RBL checking                  |
| `RBLLookup.pm`   | RBL lookup                    |
| `RegexMain.pm`   | Regex pattern matching        |
| `Sanity.pm`      | System validation             |
| `Sendmail.pm`    | Email sending                 |
| `ServerCheck.pm` | Server monitoring             |
| `ServerStats.pm` | Statistics collection         |
| `Service.pm`     | Service management            |
| `Slurp.pm`       | File reading                  |
| `URLGet.pm`      | URL fetching                  |
| `cseUI.pm`       | CSE UI components             |

---

## Modified Files - Configuration Files

### Platform-Specific Configurations

All platform configs have been modified with formatting updates and new options:

| File                   | Platform          |
| ---------------------- | ----------------- |
| `csf.cwp.conf`         | Control Web Panel |
| `csf.cyberpanel.conf`  | CyberPanel        |
| `csf.directadmin.conf` | DirectAdmin       |
| `csf.generic.conf`     | Generic Linux     |
| `csf.interworx.conf`   | InterWorx         |
| `csf.vesta.conf`       | VestaCP           |

### Allow and Ignore Lists

| File            | Purpose                 |
| --------------- | ----------------------- |
| `csf.allow`     | IP allowlist            |
| `csf.deny`      | IP denylist             |
| `csf.ignore`    | Process ignore patterns |
| `csf.pignore`   | Port ignore patterns    |
| `csf.fignore`   | File ignore patterns    |
| `csf.rignore`   | Regex ignore patterns   |
| `csf.mignore`   | Mail ignore patterns    |
| `csf.suignore`  | SU ignore patterns      |
| `csf.logignore` | Log ignore patterns     |
| `csf.uidignore` | UID ignore patterns     |
| `csf.signore`   | Script ignore patterns  |

### Other Configuration Files

| File              | Purpose              | Changes                  |
| ----------------- | -------------------- | ------------------------ |
| `csf.blocklists`  | IP blocklist sources | Added AbuseIPDB template |
| `csf.cloudflare`  | CloudFlare IP ranges | Updated ranges           |
| `csf.rblconf`     | RBL configuration    | Updated servers          |
| `csf.logfiles`    | Log file locations   | Updated paths            |
| `csf.syslogs`     | Syslog configuration | Updated settings         |
| `csf.syslogusers` | Syslog users         | Updated users            |
| `csf.dirwatch`    | Directory watch      | Updated paths            |
| `csf.dyndns`      | Dynamic DNS          | Updated settings         |
| `csf.redirect`    | Port redirects       | Updated rules            |
| `csf.resellers`   | Reseller config      | Updated settings         |
| `csf.sips`        | Server IPs           | Updated IPs              |
| `csf.smtpauth`    | SMTP auth            | Updated settings         |

---

## Modified Files - Platform Integrations

### cPanel Integration

| File                                    | Changes                |
| --------------------------------------- | ---------------------- |
| `cpanel/csf.cgi`                        | CGI interface updates  |
| `cpanel/Driver/ConfigServercsf/META.pm` | Driver metadata        |
| `cpanel.allow`                          | cPanel allowlist       |
| `cpanel.ignore`                         | cPanel ignore patterns |
| `cpanel.comodo.allow`                   | Comodo integration     |
| `cpanel.comodo.ignore`                  | Comodo ignore patterns |

### DirectAdmin Integration

| File                | Changes                      |
| ------------------- | ---------------------------- |
| `da/` directory     | Updated images and interface |
| `csf.directadmin.*` | DirectAdmin-specific configs |

### Control Web Panel Integration

| File             | Changes              |
| ---------------- | -------------------- |
| `cwp/` directory | CWP interface        |
| `csf.cwp.*`      | CWP-specific configs |

Commit `197e93acc`: Changed branding from "CentOS Web Panel" to "Control Web Panel"

### CyberPanel Integration

| File                    | Changes                     |
| ----------------------- | --------------------------- |
| `cyberpanel/` directory | Python Django modules       |
| `csf.cyberpanel.*`      | CyberPanel-specific configs |

### InterWorx Integration

| File                   | Changes                    |
| ---------------------- | -------------------------- |
| `interworx/` directory | InterWorx interface        |
| `csf.interworx.*`      | InterWorx-specific configs |

### VestaCP Integration

| File                 | Changes                  |
| -------------------- | ------------------------ |
| `vestacp/` directory | VestaCP interface        |
| `csf.vesta.*`        | VestaCP-specific configs |

### Webmin Integration

| File                             | Changes       |
| -------------------------------- | ------------- |
| `webmin/csf/` directory          | Webmin module |
| New settings button              | `69a1c24cf`   |
| AlmaLinux/Rocky10/RedHat support | `38c4f2aff`   |

### Generic UI

| File              | Changes                    |
| ----------------- | -------------------------- |
| `ui/` directory   | Standalone HTTPS interface |
| Theme selector    | Dark & light themes        |
| SSL expired certs | Testing certificates       |

---

## Modified Files - Other Scripts

### Perl Scripts

| File                  | Changes                    |
| --------------------- | -------------------------- |
| `auto.pl`             | Auto-configuration updates |
| `auto.cwp.pl`         | CWP auto-config            |
| `auto.cyberpanel.pl`  | CyberPanel auto-config     |
| `auto.directadmin.pl` | DirectAdmin auto-config    |
| `auto.generic.pl`     | Generic auto-config        |
| `auto.interworx.pl`   | InterWorx auto-config      |
| `auto.vesta.pl`       | VestaCP auto-config        |
| `apf_stub.pl`         | APF compatibility stub     |

### Shell and C Files

| File     | Changes              |
| -------- | -------------------- |
| `csf.sh` | Main shell wrapper   |
| `csf.c`  | C language component |

### Documentation

| File            | Changes           |
| --------------- | ----------------- |
| `changelog.txt` | Updated changelog |
| `csf.1.txt`     | Man page updates  |
| `csf.help`      | Help text updates |

---

## Feature Summary by Category

### New CLI Commands

| Command        | Short | Description               | Issue |
| -------------- | ----- | ------------------------- | ----- |
| `--listports`  | `-lp` | List configured ports     | #57   |
| `--addport`    | `-ap` | Add port to firewall      | #57   |
| `--removeport` | `-rp` | Remove port from firewall | #57   |

### UI Enhancements

| Feature                  | Description                   | Issue |
| ------------------------ | ----------------------------- | ----- |
| Theme selector           | Dark & light theme support    | -     |
| Sponsor icon controls    | Hide/show sponsor icon        | #72   |
| Log refresh settings     | Configurable refresh time     | #25   |
| Login attempt display    | Show remaining login attempts | -     |
| Settings button (Webmin) | Quick access to settings      | -     |

### Security Features

| Feature                    | Description                                   |
| -------------------------- | --------------------------------------------- |
| Default credential warning | Warning when using default web UI credentials |
| Content-Security-Policy    | CSP headers for web interface                 |
| Private network blocking   | Option to block private network ranges        |

### Bug Fixes

| Fix                                | Commit      |
| ---------------------------------- | ----------- |
| TTY detection for clean CLI output | `758e1180e` |
| Color code sanitization for CWP    | `c3c1127f7` |
| UI gap in Firewall Configuration   | `365e582f3` |
| Webmin settings button JS          | `69a1c24cf` |
| DirectAdmin install error          | `6e85c7a1b` |

### New Integrations

| Integration                  | Description              | Commit      |
| ---------------------------- | ------------------------ | ----------- |
| AbuseIPDB blocklist template | IP blocklist integration | `7dbe65c90` |
| AlmaLinux support (Webmin)   | OS support               | `38c4f2aff` |
| Rocky Linux 10 support       | OS support               | `38c4f2aff` |
| RedHat support (Webmin)      | OS support               | `38c4f2aff` |

---

## Detailed Change Analysis

This section provides code-level analysis of key changes derived from commit examination.

### Port Management Commands (Issue #57)

Three new CLI commands were added for port management without manual config editing:

#### `--listports` / `-lp` (Commit `05a25350f`)

**Function:** `portsList()` - 59 lines added to `src/csf.pl`

**Implementation:**

- Reads `/etc/csf/csf.conf` and extracts `TCP_IN`, `TCP_OUT`, `UDP_IN`, `UDP_OUT` protocol lines
- Parses port lists from config format: `PROTOCOL = "port1,port2,port3"`
- Displays ports grouped by protocol with colored output (blue protocol names, yellow port values)

**Usage:** `csf --listports` or `csf -lp`

#### `--addport` / `-ap` (Commit `ac9e05a6a`)

**Function:** `portAdd()` - 162 lines added

**Implementation:**

- Accepts input format: `PROTOCOL:PORT` or `PROTOCOL=PORT` (e.g., `TCP_IN:8080`)
- Validates protocol (only `TCP_IN`, `TCP_OUT`, `UDP_IN`, `UDP_OUT` accepted)
- Checks port doesn't already exist: `$ports !~ /\b\Q$port\E\b/`
- Appends port to existing list and rewrites configuration file
- Color-coded feedback: success (green), warnings (yellow), errors (red)

**Usage:** `csf --addport TCP_IN:8080` or `csf -ap UDP_IN:5353`

#### `--removeport` / `-rp` (Commit `3ba60d17f`)

**Function:** `portRemove()` - 118 lines added

**Implementation:**

- Accepts input format: `PROTOCOL:PORT`
- Splits port list by comma delimiter
- Removes matching port using `grep { $_ ne $port }`
- Rebuilds port list: `join(",", @plist)`
- Rewrites `/etc/csf/csf.conf` with updated configuration

**Usage:** `csf --removeport TCP_IN:8080` or `csf -rp UDP_IN:5353`

### Theme System (Commit `4f3d228e3`)

**Scope:** 21 files modified across all platform directories

**CSS Architecture:**

- Converted `configserver.css` from 68 lines to 1,800+ lines with comprehensive theme support
- Implemented CSS custom properties (variables) for theming:
  - Light theme (`:root`): `--bg-color: #ffffff`, `--text-color: #111111`, `--link-color: #0077cc`
  - Dark theme (`[data-theme="dark"]`): `--bg-color: #1e1d1d`, `--text-color: #ffffff`
- Added `@keyframes` animations for fade-in and scale-in transitions

**JavaScript:** `csf.min.js` updated with 130 new lines for theme switching logic

**Files Updated:**

- `src/csf/configserver.css` and `csf.min.js`
- `src/da/images/configserver.css` and `csf.min.js`
- `src/interworx/images/configserver.css` and `csf.min.js`
- `src/ui/images/configserver.css` and `csf.min.js`
- `src/webmin/csf/images/configserver.css` and `csf.min.js`

### License and Insiders System (Commit `86ff22164`)

**New Functions in `src/csf.pl`:** 79 lines added

#### `userLicenseStatus()`

- Checks `$config{SPONSOR_LICENSE}` setting
- Makes HTTPS request to `https://license.configserver.dev/?license=${license}`
- Parses JSON response for `"valid": true` within `"message"` object
- Returns: 0 (invalid/missing) or 1 (valid)

#### `userIsInsider(optional $preCheckedLicense)`

- Validates three conditions:
  1. `SPONSOR_RELEASE_INSIDERS` config enabled (== 1)
  2. `SPONSOR_LICENSE` not empty
  3. License is valid (via `userLicenseStatus()` or pre-checked param)
- Accepts optional parameter to avoid duplicate server requests
- Returns: 0 (Stable channel) or 1 (Insiders channel)

### TTY Detection (Commit `758e1180e`)

**Changes in `doversion()` function:** 7 lines modified

**Implementation:**

```perl
my $is_tty = -t STDOUT;  # Check if output is terminal

if ( !$is_tty ) {
    # Strip all ANSI color codes for non-terminal output
    # Prevents color codes in web interfaces (CWP, etc.)
}
```

**Impact:** CSF automatically detects output context - colorized for terminals, clean for web panels.

### Output Sanitization (Commit `c3c1127f7`)

**New Helper Functions:** 78 lines added to `src/csf.pl`

#### `strip_ansi($text)`

- Removes ANSI escape sequences using regex: `s/\e\[[0-9;]*[A-Za-z]//g`
- Prevents terminal manipulation attacks

#### `sanitize($text)`

- Escapes HTML special characters:
  - `&` → `&amp;`
  - `<` → `&lt;`
  - `>` → `&gt;`
  - `"` → `&quot;`
  - `'` → `&#39;`
- Prevents HTML/JavaScript injection via version strings

### Security: Default Credential Warning (Commit `6a8d569b8`)

**Scope:** 424 lines added across `src/csf.pl`, `src/lfd.pl`, `src/global.sh`

**New Logging System:**

- 40+ ANSI color escape codes defined
- Logging functions with color-coded severity:
  - `log_info()` - Blue background for informational
  - `log_warn()` - Orange background for warnings
  - `log_fail()` - Red background for errors
  - `log_pass()` - Green background for success
  - `log_debug()` - Purple background for debug

**Security Check in `dostart()`:**

```perl
if ( $config{UI_USER} eq "" or $config{UI_USER} eq "username" ) {
    log_fail( "Cannot enable CSF web interface. UI_USER has default value" );
    $config{UI} = 0;
}
elsif ( $config{UI_PASS} eq "" or $config{UI_PASS} eq "password" ) {
    log_fail( "Cannot enable CSF web interface. UI_PASS has default value" );
    $config{UI} = 0;
}
```

**Impact:** Prevents web UI from starting with insecure default credentials.

### Security: Content Security Policy (Commit `a07d9861b`)

**New Configuration Options:**

- `UI_CSP_ENABLED = "0"` - Enable/disable CSP headers
- `UI_CSP_ADVANCED_ENABLED = "0"` - Enable custom CSP rules
- `UI_CSP_ADVANCED_RULE` - Custom CSP rule template

**Default CSP Directives:**

```text
default-src 'none';
img-src 'self' data: https://*.[HOSTNAME] https://*.[HOSTIP];
script-src 'self' 'unsafe-inline';
style-src 'self' 'unsafe-inline' https://fonts.googleapis.com;
form-action 'self';
font-src 'self' https://fonts.gstatic.com;
```

**Template Variables:** `[HOSTNAME]`, `[HOSTIP]` for dynamic rules

**Protection:** Prevents XSS, data injection, and clickjacking attacks (OWASP A03:2021, A07:2021).

### Security: Private Network Blocking (Commit `915bd564c`)

**New Configuration Option:** `UI_BLOCK_PRIVATE_NET = "1"` (enabled by default)

**Blocked Ranges:**

- `192.168.x.x` (Class C private)
- `172.16-31.x.x` (Class B private)
- `10.x.x.x` (Class A private)
- Docker/virtual bridge networks

**Impact:** Prevents unauthorized access via local interface IPs and container escape attacks.

### AbuseIPDB Integration (Commit `7dbe65c90`)

**File Modified:** `src/csf.blocklists` - 16 lines added

**Template Configuration:**

```text
ABUSEIPDB|86400|10000|https://api.abuseipdb.com/api/v2/blacklist?key=YOUR_API_KEY&plaintext
```

**Format:**

- `86400` - Update interval (1 day)
- `10000` - Minimum abuse score threshold
- URL requires user's API key replacement

**Impact:** Enables integration with AbuseIPDB threat intelligence for automated blocking of known malicious IPs.

### AlmaLinux/Rocky10/RedHat Support (Commit `38c4f2aff`)

**Files Modified:** 7 files (`src/global.sh` + all install scripts)

**Path Detection:**

```bash
CSF_WEBMIN_SHARE_HOME="/usr/share/webmin"      # Debian, Ubuntu, ZorinOS
CSF_WEBMIN_LIBEXEC_HOME="/usr/libexec/webmin"  # AlmaLinux, RedHat, Rocky 10
```

**Installation Logic:** Checks both paths and installs to correct location based on OS.

**Impact:** Resolves Webmin module installation failures on RHEL-based systems.

### UI: Log Refresh Controls (Commit `80dd350a2`)

**New Configuration Options:**

- `UI_LOGS_REFRESH_TIME = "6"` - Seconds between automatic refreshes
- `UI_LOGS_START_PAUSED = "0"` - Whether logs start paused on page load

**JavaScript Updates in `csfajaxtail.js`:**

- Reads `csfStartPaused` variable from page
- Uses `setInterval()` with 1000ms cycle
- Respects pause flag before countdown
- Pause button shows "Pause" or "Continue" based on state

### UI: Sponsor Visibility Controls (Commits `f8f7f0d03`, `2a061110e`, `185654edc`)

**Configuration Options:**

- `SPONSOR_HIDE_ICON = "0"` - Hide sponsor icon in footer
- `SPONSOR_LICENSE` - If set, sponsor button hidden automatically

**DisplayUI.pm Logic:**

```perl
print "<button id='btn-sponsor'...></button>"
    if !length( $config{SPONSOR_LICENSE} // '' )
    && ( ( $config{UI_SPONSOR_HIDE} // '' ) ne '1' );
```

**Additional Change:** Removed beating heart animation from sponsor icon (class `heart` removed from CSS).

### UI: Login Failure Notification (Commit `21338f61b`)

**New Configuration Option:** `UI_RETRY_SHOW_REMAINING = "0"`

**Behavior:**

- Shows notification when login fails
- If enabled, displays count of remaining attempts before lockout
- Helps users understand brute-force protection is active

### UI: Firewall Configuration Gap Fix (Commit `365e582f3`)

**Issue:** Extra vertical gaps appearing between first and second lines in the Firewall Configuration web interface.

**Fix:**

- First line: `print "$hl<br>";` (no trailing newline)
- Subsequent lines: `print "$hl<br>\n";` (with trailing newline)
- Added URL detection to convert links to clickable `<a>` tags with `target="_blank"`
- Applied `white-space: pre-wrap; font-family: monospace; line-height: 1.2em;` styling

---

## Configuration Options Reference

All new configuration options added by the Aetherinox fork:

| Setting                   | Default | Description                                      | Issue |
| ------------------------- | ------- | ------------------------------------------------ | ----- |
| `UI_LOGS_REFRESH_TIME`    | `"6"`   | Seconds between automatic log refreshes          | #25   |
| `UI_LOGS_START_PAUSED`    | `"0"`   | Start with logs paused (1) or running (0)        | #25   |
| `UI_RETRY_SHOW_REMAINING` | `"0"`   | Show remaining login attempts after failure      | -     |
| `UI_BLOCK_PRIVATE_NET`    | `"1"`   | Block login from private network ranges          | -     |
| `UI_CSP_ENABLED`          | `"0"`   | Enable Content-Security-Policy headers           | -     |
| `UI_CSP_ADVANCED_ENABLED` | `"0"`   | Enable custom CSP rules                          | -     |
| `UI_CSP_ADVANCED_RULE`    | `""`    | Custom CSP rule with template variable support   | -     |
| `SPONSOR_HIDE_ICON`       | `"0"`   | Hide sponsor icon in footer                      | #72   |
| `SPONSOR_LICENSE`         | `""`    | License key (hides sponsor if set)               | -     |
| `SPONSOR_RELEASE_INSIDERS`| `"0"`   | Enable Insiders release channel                  | -     |

---

## Commit Reference

Base sync commit: `718dddcfa` - Initial sync from official CSF v15.00

Key feature commits:

- `4f3d228e3` - Theme selector (dark/light) - 21 files, +7,231 lines
- `05a25350f` - Port listing command (`--listports/-lp`) - +59 lines
- `3ba60d17f` - Port removal command (`--removeport/-rp`) - +118 lines
- `ac9e05a6a` - Port addition command (`--addport/-ap`) - +162 lines
- `86ff22164` - License and insiders functions - +79 lines
- `f8f7f0d03` - Sponsor hide icon setting - 8 files
- `7dbe65c90` - AbuseIPDB blocklist template - +16 lines
- `38c4f2aff` - AlmaLinux/Rocky10/RedHat support - 7 files

Security commits:

- `6a8d569b8` - Default credential warning - 3 files, +424 lines
- `a07d9861b` - Content-Security-Policy headers - 7 files
- `915bd564c` - Private network blocking - 7 files
- `c3c1127f7` - Output sanitization functions - +78 lines
- `758e1180e` - TTY detection for safe output - +7 lines

UI commits:

- `365e582f3` - Comment formatting fix
- `69a1c24cf` - Webmin settings button
- `80dd350a2` - Log refresh controls
- `21338f61b` - Login failure notification
- `2a061110e` - Sponsor button conditional display
- `185654edc` - Remove heart animation

---

Last updated: 2025-12-18
