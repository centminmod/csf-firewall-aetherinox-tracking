# Aetherinox CSF Firewall Fork - Change Documentation

This document tracks all changes between the official CSF Firewall v15.00 (GPLv3) and the Aetherinox fork.

## Summary

| Category          | Count |
| ----------------- | ----- |
| Modified files    | 168   |
| New files         | 46    |
| Files removed     | 0     |
| Total differences | 214   |

**Fork Repository:** <https://github.com/Aetherinox/csf-firewall>

**Official CSF Repository:** <https://github.com/centminmod/configserver-scripts>

---

## Repository State (as of 2026-07-05)

| Repository | HEAD Commit | Date | Message |
|------------|-------------|------|---------|
| Official CSF | [`4793f7c`](https://github.com/centminmod/configserver-scripts/commit/4793f7c) | 2025-12-20 | update readme |
| Aetherinox Fork | [`da3f5c13e`](https://github.com/Aetherinox/csf-firewall/commit/da3f5c13e) | 2026-06-16 | refactor(lfd): implement better logging |

**History rewrite (2026-02):** the fork rewrote its git history around February 2026;
every rewritten commit carries a `Former-commit-id:` trailer pointing at its
pre-rewrite hash. All commit hashes and links in this document were remapped to the
rewritten (current) hashes on 2026-07-05. The pre-rewrite history is preserved locally
under the `backup-fork-premirror` tag (old HEAD `f84e91111`, 2026-01-29).

---

## Release History

The Aetherinox fork maintains versioned releases. See [all releases](https://github.com/Aetherinox/csf-firewall/tags).

| Version | Date | Commit |
|---------|------|--------|
| [15.10](https://github.com/Aetherinox/csf-firewall/releases/tag/15.10) | 2026-02-28 | [`4260bc811`](https://github.com/Aetherinox/csf-firewall/commit/4260bc811) |
| [15.09](https://github.com/Aetherinox/csf-firewall/releases/tag/15.09) | 2026-02-23 | [`ba68270c4`](https://github.com/Aetherinox/csf-firewall/commit/ba68270c4) |
| [15.08](https://github.com/Aetherinox/csf-firewall/releases/tag/15.08) | 2025-12-13 | [`0c91771d4`](https://github.com/Aetherinox/csf-firewall/commit/0c91771d4) |
| [15.07](https://github.com/Aetherinox/csf-firewall/releases/tag/15.07) | 2025-10-24 | [`37aa56ea0`](https://github.com/Aetherinox/csf-firewall/commit/37aa56ea0) |
| [15.06](https://github.com/Aetherinox/csf-firewall/releases/tag/15.06) | 2025-10-16 | [`917d74ae3`](https://github.com/Aetherinox/csf-firewall/commit/917d74ae3) |
| [15.05](https://github.com/Aetherinox/csf-firewall/releases/tag/15.05) | 2025-10-16 | [`8f5fe75ba`](https://github.com/Aetherinox/csf-firewall/commit/8f5fe75ba) |
| [15.04](https://github.com/Aetherinox/csf-firewall/releases/tag/15.04) | 2025-10-15 | [`e71a363a9`](https://github.com/Aetherinox/csf-firewall/commit/e71a363a9) |
| [15.03](https://github.com/Aetherinox/csf-firewall/releases/tag/15.03) | 2025-10-15 | [`f736468b4`](https://github.com/Aetherinox/csf-firewall/commit/f736468b4) |
| [15.02](https://github.com/Aetherinox/csf-firewall/releases/tag/15.02) | 2025-10-14 | [`4cf2f2089`](https://github.com/Aetherinox/csf-firewall/commit/4cf2f2089) |
| [15.01](https://github.com/Aetherinox/csf-firewall/releases/tag/15.01) | 2025-10-14 | [`4cf2f2089`](https://github.com/Aetherinox/csf-firewall/commit/4cf2f2089) |
| [15.00](https://github.com/Aetherinox/csf-firewall/releases/tag/15.00) | 2025-10-14 | [`220189209`](https://github.com/Aetherinox/csf-firewall/commit/220189209) |

---

## Change Statistics

| Metric            | Value      |
| ----------------- | ---------- |
| Lines added       | 84,072     |
| Lines removed     | 33,448     |
| Net change        | +50,624    |
| Fork size (differing files only) | 13,532 KB  |
| Official size (differing files only) | 2,917 KB   |
| Size difference   | +10,616 KB |

Note: size figures sum only the modified and new files compared between trees
(full-tree byte totals are ~19,189 KB fork vs ~8,573 KB official).

### Most Changed Files (by commit count)

| Rank | File                                | Commits |
| ---- | ----------------------------------- | ------- |
| 1    | `ConfigServer/DisplayUI.pm`         | 54      |
| 2    | `ConfigServer/ServerCheck.pm`       | 19      |
| 3    | `ConfigServer/Config.pm`            | 15      |
| 4    | `ConfigServer/RBLCheck.pm`          | 13      |
| 5    | `ConfigServer/RegexMain.pm`         | 9       |
| 6    | `ConfigServer/DisplayResellerUI.pm` | 8       |
| 7    | `ConfigServer/Messenger.pm`         | 8       |
| 8    | `ConfigServer/Sanity.pm`            | 8       |
| 9    | `ConfigServer/AbuseIP.pm`           | 7       |
| 10   | `ConfigServer/CheckIP.pm`           | 6       |

---

## New Files (46 files)

Files that exist only in the Aetherinox fork.

### New Perl Modules

| File | Description | Initial Commit |
|------|-------------|----------------|
| `csf-firewall-aetherinox/src/ConfigServer/JSON.pm` | Bundled JSON encode/decode module (used by sponsor/license functions) | [`7f8a50ffb`](https://github.com/Aetherinox/csf-firewall/commit/7f8a50ffb) |
| `csf-firewall-aetherinox/src/ConfigServer/Packages.pm` | Package/dependency handling module | [`858da7be3`](https://github.com/Aetherinox/csf-firewall/commit/858da7be3) |
| `csf-firewall-aetherinox/src/ConfigServer/Perl/URI.pm` | Bundled `URI::Escape` (drops external module requirement) | [`417a7e91a`](https://github.com/Aetherinox/csf-firewall/commit/417a7e91a) |
| `csf-firewall-aetherinox/src/ConfigServer/Sanitize.pm` | Output sanitization helpers (`html_escape`, `strip_ansi`) | [`7a8a80e6b`](https://github.com/Aetherinox/csf-firewall/commit/7a8a80e6b) |

### Dark Theme Sprite Assets (10 files)

Dark-theme variants of the chosen-select sprite, added by commit
[`4d6f4f098`](https://github.com/Aetherinox/csf-firewall/commit/4d6f4f098) to all five
platform image directories (`csf/`, `da/images/`, `interworx/images/`, `ui/images/`,
`webmin/csf/images/`):

| File | Description |
|------|-------------|
| `chosen-sprite-w.png` | Dark theme sprite (×5 directories) |
| `chosen-sprite@2x-w.png` | Dark theme sprite, retina (×5 directories) |

### Branding Assets

| File | Description | Initial Commit |
|------|-------------|----------------|
| `csf-firewall-aetherinox/src/csf/csf-logo.svg` | Main CSF logo (SVG) | [`035672e46`](https://github.com/Aetherinox/csf-firewall/commit/035672e46) |
| `csf-firewall-aetherinox/src/csf/csf-logo-alt.svg` | Alternate CSF logo (SVG) | [`035672e46`](https://github.com/Aetherinox/csf-firewall/commit/035672e46) |
| `csf-firewall-aetherinox/src/csf/csf.png` | CSF logo (PNG) | [`62743b25d`](https://github.com/Aetherinox/csf-firewall/commit/62743b25d) |
| `csf-firewall-aetherinox/src/da/images/csf-logo.svg` | DirectAdmin logo | [`035672e46`](https://github.com/Aetherinox/csf-firewall/commit/035672e46) |
| `csf-firewall-aetherinox/src/da/images/csf-logo-alt.svg` | DirectAdmin alt logo | [`035672e46`](https://github.com/Aetherinox/csf-firewall/commit/035672e46) |
| `csf-firewall-aetherinox/src/da/images/csf.png` | DirectAdmin logo PNG | [`62743b25d`](https://github.com/Aetherinox/csf-firewall/commit/62743b25d) |
| `csf-firewall-aetherinox/src/interworx/images/csf-logo.svg` | InterWorx logo | [`035672e46`](https://github.com/Aetherinox/csf-firewall/commit/035672e46) |
| `csf-firewall-aetherinox/src/interworx/images/csf-logo-alt.svg` | InterWorx alt logo | [`035672e46`](https://github.com/Aetherinox/csf-firewall/commit/035672e46) |
| `csf-firewall-aetherinox/src/interworx/images/csf.png` | InterWorx logo PNG | [`62743b25d`](https://github.com/Aetherinox/csf-firewall/commit/62743b25d) |
| `csf-firewall-aetherinox/src/ui/images/csf-logo.svg` | Generic UI logo | [`035672e46`](https://github.com/Aetherinox/csf-firewall/commit/035672e46) |
| `csf-firewall-aetherinox/src/ui/images/csf-logo-alt.svg` | Generic UI alt logo | [`035672e46`](https://github.com/Aetherinox/csf-firewall/commit/035672e46) |
| `csf-firewall-aetherinox/src/ui/images/csf.png` | Generic UI logo PNG | [`62743b25d`](https://github.com/Aetherinox/csf-firewall/commit/62743b25d) |
| `csf-firewall-aetherinox/src/webmin/csf/images/csf-logo.svg` | Webmin logo | [`1baf83b4f`](https://github.com/Aetherinox/csf-firewall/commit/1baf83b4f) |
| `csf-firewall-aetherinox/src/webmin/csf/images/csf-logo-alt.svg` | Webmin alt logo | [`1baf83b4f`](https://github.com/Aetherinox/csf-firewall/commit/1baf83b4f) |
| `csf-firewall-aetherinox/src/webmin/csf/images/csf.png` | Webmin logo PNG | [`62743b25d`](https://github.com/Aetherinox/csf-firewall/commit/62743b25d) |

### JavaScript Assets

| File | Description | Initial Commit |
|------|-------------|----------------|
| `csf-firewall-aetherinox/src/csf/csf.min.js` | Minified CSF JS | [`12f9e1afc`](https://github.com/Aetherinox/csf-firewall/commit/12f9e1afc) |
| `csf-firewall-aetherinox/src/csf/csfont.min.js` | Font JavaScript | [`12c9f7c1f`](https://github.com/Aetherinox/csf-firewall/commit/12c9f7c1f) |
| `csf-firewall-aetherinox/src/da/images/csf.min.js` | DirectAdmin JS | [`12f9e1afc`](https://github.com/Aetherinox/csf-firewall/commit/12f9e1afc) |
| `csf-firewall-aetherinox/src/da/images/csfont.min.js` | DirectAdmin font JS | [`12c9f7c1f`](https://github.com/Aetherinox/csf-firewall/commit/12c9f7c1f) |
| `csf-firewall-aetherinox/src/interworx/images/csf.min.js` | InterWorx JS | [`12f9e1afc`](https://github.com/Aetherinox/csf-firewall/commit/12f9e1afc) |
| `csf-firewall-aetherinox/src/interworx/images/csfont.min.js` | InterWorx font JS | [`12c9f7c1f`](https://github.com/Aetherinox/csf-firewall/commit/12c9f7c1f) |
| `csf-firewall-aetherinox/src/ui/images/csf.min.js` | Generic UI JS | [`12f9e1afc`](https://github.com/Aetherinox/csf-firewall/commit/12f9e1afc) |
| `csf-firewall-aetherinox/src/ui/images/csfont.min.js` | Generic UI font JS | [`12c9f7c1f`](https://github.com/Aetherinox/csf-firewall/commit/12c9f7c1f) |
| `csf-firewall-aetherinox/src/webmin/csf/images/csf.min.js` | Webmin JS | [`12f9e1afc`](https://github.com/Aetherinox/csf-firewall/commit/12f9e1afc) |
| `csf-firewall-aetherinox/src/webmin/csf/images/csfont.min.js` | Webmin font JS | [`12c9f7c1f`](https://github.com/Aetherinox/csf-firewall/commit/12c9f7c1f) |

### New Shell Scripts

| File | Description | Initial Commit |
|------|-------------|----------------|
| `csf-firewall-aetherinox/src/csfpre.sh` | Pre-firewall hook script | [`62743b25d`](https://github.com/Aetherinox/csf-firewall/commit/62743b25d) |
| `csf-firewall-aetherinox/src/csfpost.sh` | Post-firewall hook script | [`62743b25d`](https://github.com/Aetherinox/csf-firewall/commit/62743b25d) |
| `csf-firewall-aetherinox/src/global.sh` | Global shell functions | [`7cb0d366a`](https://github.com/Aetherinox/csf-firewall/commit/7cb0d366a) |

### Configuration and SSL

| File | Description | Initial Commit |
|------|-------------|----------------|
| `csf-firewall-aetherinox/src/regex.txt` | Custom regex patterns | [`62743b25d`](https://github.com/Aetherinox/csf-firewall/commit/62743b25d) |
| `csf-firewall-aetherinox/src/defaults.txt` | Default values reference consumed by `ConfigServer::Config` | [`51f365ddb`](https://github.com/Aetherinox/csf-firewall/commit/51f365ddb) |
| `csf-firewall-aetherinox/src/ui/ssl-expired/server.crt` | Expired SSL cert (testing) | [`cd4a42bc4`](https://github.com/Aetherinox/csf-firewall/commit/cd4a42bc4) |
| `csf-firewall-aetherinox/src/ui/ssl-expired/server.key` | Expired SSL key (testing) | [`cd4a42bc4`](https://github.com/Aetherinox/csf-firewall/commit/cd4a42bc4) |

---

## Modified Files - Core Scripts

### csf.pl (Main Firewall Script)

**Path:** `csf-firewall-aetherinox/src/csf.pl`

**Commit History (Recent):**

| Commit      | Description                                                                              |
| ----------- | ---------------------------------------------------------------------------------------- |
| [`8853f98f5`](https://github.com/Aetherinox/csf-firewall/commit/8853f98f5) | fix(ui): incorrectly adding gap between first and second line in web interface           |
| [`77df09930`](https://github.com/Aetherinox/csf-firewall/commit/77df09930) | fix(cli): detect tty for colored or clean output in responses                            |
| [`1037e4d8a`](https://github.com/Aetherinox/csf-firewall/commit/1037e4d8a) | fix(cwp): sanitize and strip color codes for cwp version status                          |
| [`814c0033c`](https://github.com/Aetherinox/csf-firewall/commit/814c0033c) | chore(csf): update log functionality output for users                                    |
| [`d5350157a`](https://github.com/Aetherinox/csf-firewall/commit/d5350157a) | style(csf): clean up command dictionary                                                  |
| [`c876be73c`](https://github.com/Aetherinox/csf-firewall/commit/c876be73c) | feat(license): add new funcs for license and insiders checks                             |
| [`ae88914a3`](https://github.com/Aetherinox/csf-firewall/commit/ae88914a3) | feat(cli): add command `--listports`, `-lp` #57                                          |
| [`5ccd44f17`](https://github.com/Aetherinox/csf-firewall/commit/5ccd44f17) | feat(cli): add command `--removeport`, `-rp` #57                                         |
| [`93055acc3`](https://github.com/Aetherinox/csf-firewall/commit/93055acc3) | feat(cli): add command `--addport`, `-ap` #57                                            |
| [`ee56d70ec`](https://github.com/Aetherinox/csf-firewall/commit/ee56d70ec) | refactor(csf): update module output for updates                                          |
| [`ac61b07ca`](https://github.com/Aetherinox/csf-firewall/commit/ac61b07ca) | feat(csf): add warning to console output when using default web ui username and password |

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
| [`43ce1c956`](https://github.com/Aetherinox/csf-firewall/commit/43ce1c956) | refactor(generic): update interface header                                               |
| [`ac61b07ca`](https://github.com/Aetherinox/csf-firewall/commit/ac61b07ca) | feat(csf): add warning to console output when using default web ui username and password |

**Key Changes:**

- Security warning for default credentials
- Interface header refactoring with structured HTML layout (header-left/header-right divs)

### csf.conf (Main Configuration)

**Path:** `csf-firewall-aetherinox/src/csf.conf`

**Commit History (Recent):**

| Commit      | Description                                                                               |
| ----------- | ----------------------------------------------------------------------------------------- |
| [`0fa1f0428`](https://github.com/Aetherinox/csf-firewall/commit/0fa1f0428) | feat(sponsor): update default value for sponsor setting `SPONSOR_ICON_ANIM`               |
| [`bd625f7f9`](https://github.com/Aetherinox/csf-firewall/commit/bd625f7f9) | feat(ui): add new setting `SPONSOR_HIDE_ICON` #72                                         |
| [`30c34c9ad`](https://github.com/Aetherinox/csf-firewall/commit/30c34c9ad) | style(generic): update formatting                                                         |
| [`4f7fb1a21`](https://github.com/Aetherinox/csf-firewall/commit/4f7fb1a21) | chore: add input value type to LF_MODSEC_PERM comments #59                                |
| [`ce875faf3`](https://github.com/Aetherinox/csf-firewall/commit/ce875faf3) | chore: update config description for `LF_MODSEC` #59                                      |
| [`e394cca24`](https://github.com/Aetherinox/csf-firewall/commit/e394cca24) | feat: add insiders config items                                                           |
| [`f01c2abcc`](https://github.com/Aetherinox/csf-firewall/commit/f01c2abcc) | feat(ui): add highlighter classes "Firewall Configuration" page                           |
| [`b47dd03a8`](https://github.com/Aetherinox/csf-firewall/commit/b47dd03a8) | feat(ui): add two settings: `UI_LOGS_REFRESH_TIME` and `UI_LOGS_START_PAUSED` #25         |
| [`a39ab335f`](https://github.com/Aetherinox/csf-firewall/commit/a39ab335f) | refactor(conf): format comments for web interface                                         |
| [`37401ee0c`](https://github.com/Aetherinox/csf-firewall/commit/37401ee0c) | feat: add content-security-policy to web interface; new settings                          |
| [`1498fa5f9`](https://github.com/Aetherinox/csf-firewall/commit/1498fa5f9) | feat: add login failure notification to login page; new setting `UI_RETRY_SHOW_REMAINING` |
| [`179ce1355`](https://github.com/Aetherinox/csf-firewall/commit/179ce1355) | chore(conf): update configs                                                               |
| [`30405bcff`](https://github.com/Aetherinox/csf-firewall/commit/30405bcff) | feat: add new `csf.conf` setting `UI_BLOCK_PRIVATE_NET`                                   |
| [`4eef2bfe3`](https://github.com/Aetherinox/csf-firewall/commit/4eef2bfe3) | feat: add env var `UI_LOGS_REFRESH`                                                       |
| [`e10d53ef3`](https://github.com/Aetherinox/csf-firewall/commit/e10d53ef3) | feat: add env var `UI_BLOCK_PRIVATE_NET`                                                  |

**New Configuration Options:**

| Setting                   | Description                   | Issue |
| ------------------------- | ----------------------------- | ----- |
| `SPONSOR_ICON_ANIM`       | Enable sponsor icon animation | -     |
| `SPONSOR_ICON_HIDE`       | Hide sponsor icon in UI (added as `SPONSOR_HIDE_ICON` in [`bd625f7f9`](https://github.com/Aetherinox/csf-firewall/commit/bd625f7f9), renamed in [`0fa1f0428`](https://github.com/Aetherinox/csf-firewall/commit/0fa1f0428)) | #72   |
| `UI_LOGS_REFRESH_TIME`    | Log refresh interval          | #25   |
| `UI_LOGS_START_PAUSED`    | Start with logs paused        | #25   |
| `UI_RETRY_SHOW_REMAINING` | Show remaining login attempts | -     |
| `UI_BLOCK_PRIVATE_NET`    | Block private network ranges  | -     |
| `UI_LOGS_REFRESH`         | Log refresh toggle            | -     |
| `UI_WEBMIN_SHOW_BUTTON_CONFIG` | Show config button in Webmin module ([`a51a077ab`](https://github.com/Aetherinox/csf-firewall/commit/a51a077ab)) | -     |

---

## Modified Files - ConfigServer Modules (24 files)

All Perl modules in `csf-firewall-aetherinox/src/ConfigServer/` directory.

### DisplayUI.pm (Web Interface)

**Commit History:**

| Commit      | Description                                                                                |
| ----------- | ------------------------------------------------------------------------------------------ |
| [`edece43f6`](https://github.com/Aetherinox/csf-firewall/commit/edece43f6) | fix(ui): harden sponsor functionality, eliminate client-side trust                         |
| [`d85665f70`](https://github.com/Aetherinox/csf-firewall/commit/d85665f70) | fix(ui): sanitize UI, use `textContent` instead of `innerHTML`                             |
| [`c95f9ae80`](https://github.com/Aetherinox/csf-firewall/commit/c95f9ae80) | chore(ui): remove external dependency                                                      |
| [`2afe04d9f`](https://github.com/Aetherinox/csf-firewall/commit/2afe04d9f) | style(ui): conformity                                                                      |
| [`1661d87e5`](https://github.com/Aetherinox/csf-firewall/commit/1661d87e5) | fix(interworx): correct vertical scrollbar showing in iframe                              |
| [`015a69e65`](https://github.com/Aetherinox/csf-firewall/commit/015a69e65) | fix(cyberpanel): correct issue with iframe showing small vertical scrollbar               |
| [`1f33294d8`](https://github.com/Aetherinox/csf-firewall/commit/1f33294d8) | fix(cyberpanel): fix footer padding for cyberpanel                                         |
| [`c73b72a1e`](https://github.com/Aetherinox/csf-firewall/commit/c73b72a1e) | feat(ui): add new class tag `value-restricted`, `value-disabled`                           |
| [`522fcc616`](https://github.com/Aetherinox/csf-firewall/commit/522fcc616) | feat(cyberpanel): enable new footer with theme selector                                    |
| [`69e172605`](https://github.com/Aetherinox/csf-firewall/commit/69e172605) | feat(cwp): enable new footer for `control web panel`                                       |
| [`54a924443`](https://github.com/Aetherinox/csf-firewall/commit/54a924443) | feat(directadmin): enable new footer for `directadmin`                                     |
| [`fd0bb6db4`](https://github.com/Aetherinox/csf-firewall/commit/fd0bb6db4) | fix(ui): force homepage buttons to have same width                                         |
| [`452ed724d`](https://github.com/Aetherinox/csf-firewall/commit/452ed724d) | fix(ui): proper formatting for each section in gui config editor                           |
| [`0fa1f0428`](https://github.com/Aetherinox/csf-firewall/commit/0fa1f0428) | feat(sponsor): update default value for sponsor setting `SPONSOR_ICON_ANIM`                |
| [`8853f98f5`](https://github.com/Aetherinox/csf-firewall/commit/8853f98f5) | fix(ui): incorrectly adding gap between first and second line in web interface             |
| [`df6dc4651`](https://github.com/Aetherinox/csf-firewall/commit/df6dc4651) | fix(webmin): add webmin `settings` button to interface without breaking theme js           |
| [`70f5a8db7`](https://github.com/Aetherinox/csf-firewall/commit/70f5a8db7) | fix(webmin): ensure each setting is properly formatted, pre-wrap descriptions              |
| [`bd625f7f9`](https://github.com/Aetherinox/csf-firewall/commit/bd625f7f9) | feat(ui): add new setting `SPONSOR_HIDE_ICON` #72                                          |
| [`aecdc1cfc`](https://github.com/Aetherinox/csf-firewall/commit/aecdc1cfc) | feat(ui): hide sponsor button if `SPONSOR_LICENSE` specified, or `UI_SPONSOR_HIDE = 1` #72 |
| [`66402705a`](https://github.com/Aetherinox/csf-firewall/commit/66402705a) | feat(ui): remove beating heart animation for sponsor icon #72                              |

**Key Changes:**

- Homepage button width consistency
- GUI config editor section formatting
- Sponsor icon animation setting
- Sponsor icon visibility controls
- New footer with theme selector for CyberPanel, CWP, DirectAdmin
- CSS class tags: `value-restricted`, `value-disabled`
- Iframe scrollbar fixes for InterWorx and CyberPanel
- Webmin settings button integration
- UI formatting fixes
- Setting description formatting
- Hardened sponsor functionality (eliminate client-side trust)
- UI sanitization (use `textContent` over `innerHTML`)

### DisplayResellerUI.pm

**Changes:** Reseller UI modifications paralleling DisplayUI.pm changes

### AbuseIP.pm

**Commit History:**

| Commit      | Description                                                                  |
| ----------- | ---------------------------------------------------------------------------- |
| [`2fce6ccb6`](https://github.com/Aetherinox/csf-firewall/commit/2fce6ccb6) | chore: update csf main repo for `v15.01` server changes                      |
| [`a6a6f93a1`](https://github.com/Aetherinox/csf-firewall/commit/a6a6f93a1) | refactor: update headers, commenting in config files, line length conformity |

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

Commit [`ea9c86b60`](https://github.com/Aetherinox/csf-firewall/commit/ea9c86b60): Changed branding from "CentOS Web Panel" to "Control Web Panel"

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
| New settings button              | [`df6dc4651`](https://github.com/Aetherinox/csf-firewall/commit/df6dc4651)   |
| AlmaLinux/Rocky10/RedHat support | [`036eccb34`](https://github.com/Aetherinox/csf-firewall/commit/036eccb34)   |

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

| File                        | Changes                                              |
| --------------------------- | ---------------------------------------------------- |
| `csf.sh`                    | Main shell wrapper                                   |
| `csf.c`                     | C language component                                 |
| `extras/scripts/docker.sh`  | Docker integration script rewrite (+1692/-960 lines) |
| `extras/scripts/openvpn.sh` | OpenVPN integration script rewrite                   |
| `global.sh`                 | POSIX compliancy refactoring (+102/-441 lines)       |
| `csfpre.sh`                 | POSIX compliancy refactoring                         |
| `csfpost.sh`                | POSIX compliancy refactoring                         |

### Documentation

| File            | Changes                                                                                                    |
| --------------- | ---------------------------------------------------------------------------------------------------------- |
| `changelog.txt` | Updated changelog; 15.09 release notes added ([`7e8ee2f3f`](https://github.com/Aetherinox/csf-firewall/commit/7e8ee2f3f)) |
| `csf.1.txt`     | Man page updates                                                                                           |
| `csf.help`      | Help text updates                                                                                          |

---

## Feature Summary by Category

### New CLI Commands

| Command        | Short | Description               | Issue |
| -------------- | ----- | ------------------------- | ----- |
| `--listports`  | `-lp` | List configured ports     | #57   |
| `--addport`    | `-ap` | Add port to firewall      | #57   |
| `--removeport` | `-rp` | Remove port from firewall | #57   |

### UI Enhancements

| Feature                     | Description                            | Issue |
| --------------------------- | -------------------------------------- | ----- |
| Theme selector              | Dark & light theme support             | -     |
| CyberPanel footer           | New footer with theme selector         | -     |
| CWP footer                  | New footer for Control Web Panel       | -     |
| DirectAdmin footer          | New footer for DirectAdmin             | -     |
| CSS class tags              | `value-restricted`, `value-disabled`   | -     |
| Sponsor icon controls       | Hide/show sponsor icon                 | #72   |
| Log refresh settings        | Configurable refresh time              | #25   |
| Login attempt display       | Show remaining login attempts          | -     |
| Settings button (Webmin)    | Quick access to settings               | -     |

### Security Features

| Feature                      | Description                                              |
| ---------------------------- | -------------------------------------------------------- |
| Default credential warning   | Warning when using default web UI credentials            |
| Content-Security-Policy      | CSP headers for web interface                            |
| Private network blocking     | Option to block private network ranges                   |
| Sponsor hardening            | Eliminate client-side trust in sponsor functionality     |
| UI sanitization              | Use `textContent` instead of `innerHTML` to prevent XSS  |

### Bug Fixes

| Fix                                      | Commit      |
| ---------------------------------------- | ----------- |
| InterWorx iframe vertical scrollbar      | [`1661d87e5`](https://github.com/Aetherinox/csf-firewall/commit/1661d87e5) |
| CyberPanel iframe vertical scrollbar     | [`015a69e65`](https://github.com/Aetherinox/csf-firewall/commit/015a69e65) |
| CyberPanel footer padding                | [`1f33294d8`](https://github.com/Aetherinox/csf-firewall/commit/1f33294d8) |
| Homepage buttons same width              | [`fd0bb6db4`](https://github.com/Aetherinox/csf-firewall/commit/fd0bb6db4) |
| GUI config editor formatting             | [`452ed724d`](https://github.com/Aetherinox/csf-firewall/commit/452ed724d) |
| TTY detection for clean CLI output       | [`77df09930`](https://github.com/Aetherinox/csf-firewall/commit/77df09930) |
| Color code sanitization for CWP          | [`1037e4d8a`](https://github.com/Aetherinox/csf-firewall/commit/1037e4d8a) |
| UI gap in Firewall Configuration         | [`8853f98f5`](https://github.com/Aetherinox/csf-firewall/commit/8853f98f5) |
| Webmin settings button JS                | [`df6dc4651`](https://github.com/Aetherinox/csf-firewall/commit/df6dc4651) |
| DirectAdmin install error                | [`e8254d031`](https://github.com/Aetherinox/csf-firewall/commit/e8254d031) |

### New Integrations

| Integration                  | Description              | Commit      |
| ---------------------------- | ------------------------ | ----------- |
| AbuseIPDB blocklist template | IP blocklist integration | [`f2a2e5206`](https://github.com/Aetherinox/csf-firewall/commit/f2a2e5206) |
| AlmaLinux support (Webmin)   | OS support               | [`036eccb34`](https://github.com/Aetherinox/csf-firewall/commit/036eccb34) |
| Rocky Linux 10 support       | OS support               | [`036eccb34`](https://github.com/Aetherinox/csf-firewall/commit/036eccb34) |
| RedHat support (Webmin)      | OS support               | [`036eccb34`](https://github.com/Aetherinox/csf-firewall/commit/036eccb34) |

---

## Detailed Change Analysis

This section provides code-level analysis of key changes derived from commit examination.

### Port Management Commands (Issue #57)

Three new CLI commands were added for port management without manual config editing:

#### `--listports` / `-lp` (Commit [`ae88914a3`](https://github.com/Aetherinox/csf-firewall/commit/ae88914a3))

**Function:** `portsList()` - 59 lines added to `src/csf.pl`

**Implementation:**

- Reads `/etc/csf/csf.conf` and extracts `TCP_IN`, `TCP_OUT`, `UDP_IN`, `UDP_OUT` protocol lines
- Parses port lists from config format: `PROTOCOL = "port1,port2,port3"`
- Displays ports grouped by protocol with colored output (blue protocol names, yellow port values)

**Usage:** `csf --listports` or `csf -lp`

#### `--addport` / `-ap` (Commit [`93055acc3`](https://github.com/Aetherinox/csf-firewall/commit/93055acc3))

**Function:** `portAdd()` - 162 lines added

**Implementation:**

- Accepts input format: `PROTOCOL:PORT` or `PROTOCOL=PORT` (e.g., `TCP_IN:8080`)
- Validates protocol (only `TCP_IN`, `TCP_OUT`, `UDP_IN`, `UDP_OUT` accepted)
- Checks port doesn't already exist: `$ports !~ /\b\Q$port\E\b/`
- Appends port to existing list and rewrites configuration file
- Color-coded feedback: success (green), warnings (yellow), errors (red)

**Usage:** `csf --addport TCP_IN:8080` or `csf -ap UDP_IN:5353`

#### `--removeport` / `-rp` (Commit [`5ccd44f17`](https://github.com/Aetherinox/csf-firewall/commit/5ccd44f17))

**Function:** `portRemove()` - 118 lines added

**Implementation:**

- Accepts input format: `PROTOCOL:PORT`
- Splits port list by comma delimiter
- Removes matching port using `grep { $_ ne $port }`
- Rebuilds port list: `join(",", @plist)`
- Rewrites `/etc/csf/csf.conf` with updated configuration

**Usage:** `csf --removeport TCP_IN:8080` or `csf -rp UDP_IN:5353`

### Theme System (Commit [`12f9e1afc`](https://github.com/Aetherinox/csf-firewall/commit/12f9e1afc))

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

### License and Insiders System (Commit [`c876be73c`](https://github.com/Aetherinox/csf-firewall/commit/c876be73c))

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

### TTY Detection (Commit [`77df09930`](https://github.com/Aetherinox/csf-firewall/commit/77df09930))

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

### Output Sanitization (Commit [`1037e4d8a`](https://github.com/Aetherinox/csf-firewall/commit/1037e4d8a))

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

### Security: Default Credential Warning (Commit [`ac61b07ca`](https://github.com/Aetherinox/csf-firewall/commit/ac61b07ca))

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

### Security: Content Security Policy (Commit [`37401ee0c`](https://github.com/Aetherinox/csf-firewall/commit/37401ee0c))

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

### Security: Private Network Blocking (Commit [`30405bcff`](https://github.com/Aetherinox/csf-firewall/commit/30405bcff))

**New Configuration Option:** `UI_BLOCK_PRIVATE_NET = "1"` (enabled by default)

**Blocked Ranges:**

- `192.168.x.x` (Class C private)
- `172.16-31.x.x` (Class B private)
- `10.x.x.x` (Class A private)
- Docker/virtual bridge networks

**Impact:** Prevents unauthorized access via local interface IPs and container escape attacks.

### AbuseIPDB Integration (Commit [`f2a2e5206`](https://github.com/Aetherinox/csf-firewall/commit/f2a2e5206))

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

### AlmaLinux/Rocky10/RedHat Support (Commit [`036eccb34`](https://github.com/Aetherinox/csf-firewall/commit/036eccb34))

**Files Modified:** 7 files (`src/global.sh` + all install scripts)

**Path Detection:**

```bash
CSF_WEBMIN_SHARE_HOME="/usr/share/webmin"      # Debian, Ubuntu, ZorinOS
CSF_WEBMIN_LIBEXEC_HOME="/usr/libexec/webmin"  # AlmaLinux, RedHat, Rocky 10
```

**Installation Logic:** Checks both paths and installs to correct location based on OS.

**Impact:** Resolves Webmin module installation failures on RHEL-based systems.

### UI: Log Refresh Controls (Commit [`b47dd03a8`](https://github.com/Aetherinox/csf-firewall/commit/b47dd03a8))

**New Configuration Options:**

- `UI_LOGS_REFRESH_TIME = "6"` - Seconds between automatic refreshes
- `UI_LOGS_START_PAUSED = "0"` - Whether logs start paused on page load

**JavaScript Updates in `csfajaxtail.js`:**

- Reads `csfStartPaused` variable from page
- Uses `setInterval()` with 1000ms cycle
- Respects pause flag before countdown
- Pause button shows "Pause" or "Continue" based on state

### UI: Sponsor Visibility Controls (Commits [`bd625f7f9`](https://github.com/Aetherinox/csf-firewall/commit/bd625f7f9), [`aecdc1cfc`](https://github.com/Aetherinox/csf-firewall/commit/aecdc1cfc), [`66402705a`](https://github.com/Aetherinox/csf-firewall/commit/66402705a))

**Configuration Options:**

- `SPONSOR_ICON_HIDE = "0"` - Hide sponsor icon in footer (added as `SPONSOR_HIDE_ICON`, renamed in [`0fa1f0428`](https://github.com/Aetherinox/csf-firewall/commit/0fa1f0428))
- `SPONSOR_LICENSE` - If set, sponsor button hidden automatically

**DisplayUI.pm Logic (current):**

```perl
print "<button id='btn-sponsor'...></button>"
    if !length( $config{SPONSOR_LICENSE} // '' )
    && ( ( $config{SPONSOR_ICON_HIDE} // '' ) ne '1' );
```

**Additional Change:** Removed beating heart animation from sponsor icon (class `heart` removed from CSS).

### UI: Login Failure Notification (Commit [`1498fa5f9`](https://github.com/Aetherinox/csf-firewall/commit/1498fa5f9))

**New Configuration Option:** `UI_RETRY_SHOW_REMAINING = "0"`

**Behavior:**

- Shows notification when login fails
- If enabled, displays count of remaining attempts before lockout
- Helps users understand brute-force protection is active

### UI: Firewall Configuration Gap Fix (Commit [`8853f98f5`](https://github.com/Aetherinox/csf-firewall/commit/8853f98f5))

**Issue:** Extra vertical gaps appearing between first and second lines in the Firewall Configuration web interface.

**Fix:**

- First line: `print "$hl<br>";` (no trailing newline)
- Subsequent lines: `print "$hl<br>\n";` (with trailing newline)
- Added URL detection to convert links to clickable `<a>` tags with `target="_blank"`
- Applied `white-space: pre-wrap; font-family: monospace; line-height: 1.2em;` styling

### Docker Integration Script Rewrite (Commit [`65bfcd75e`](https://github.com/Aetherinox/csf-firewall/commit/65bfcd75e))

**File:** `extras/scripts/docker.sh`
**Changes:** +1,692 / -960 lines (complete rewrite)
**Purpose:** Whitelists Docker container IP addresses in CSF's allow list (`/etc/csf/csf.allow`)

**Architectural Changes:**

| Change           | Before          | After                              |
| ---------------- | --------------- | ---------------------------------- |
| Shell            | `#!/bin/bash`   | `#!/bin/sh` (POSIX compatible)     |
| Package managers | apt-get only    | apt-get, dnf, yum (multi-distro)   |
| Config syntax    | Bash arrays     | POSIX strings                      |

**New Features:**

1. **7-Level Logging System** - Color-coded severity output:
   - `verbose()` - Purple badge for verbose messages
   - `debug()` - Dark badge for debug (dev/dryrun only)
   - `info()` - Blue badge for informational
   - `ok()` - Green badge for success
   - `warn()` - Orange badge for warnings
   - `danger()` - Red badge for danger alerts
   - `error()` - Red badge for fatal errors

2. **Dryrun Mode** - `--dryrun` flag for safe testing without system changes

3. **ASCII Box Formatting** - Professional output presentation:
   - `prinb(title)` - Complete box around title
   - `princ(title)` - Cropped box (left border only)
   - `prinp(title, text)` - Multi-line paragraph box with word-wrap
   - `prin0()` - Horizontal separator line

4. **Multi-Distribution Support** - Package manager detection:

   ```bash
   if command -v apt-get >/dev/null 2>&1; then
       apt-get install -y -qq iptables
   elif command -v dnf >/dev/null 2>&1; then
       dnf install -y iptables
   elif command -v yum >/dev/null 2>&1; then
       yum install -y iptables
   fi
   ```

5. **Enhanced Validation** - `service_exists()` function checks both `/etc/init.d/` and PATH

6. **Version Tracking** - App metadata with version 15.0.9

**Backward Compatible:** Configuration variable names unchanged; only internal architecture modified

**Additional Enhancement (Commit [`aabd6bcc5`](https://github.com/Aetherinox/csf-firewall/commit/aabd6bcc5)):**

- Added command-line flag handling (+249/-164 lines)
- Extended argument parsing for runtime configuration

### OpenVPN Integration Script Rewrite (Commit [`d958f5f65`](https://github.com/Aetherinox/csf-firewall/commit/d958f5f65))

**File:** `extras/scripts/openvpn.sh`
**Changes:** +1,219 / -243 lines (complete rewrite)
**Purpose:** Configures CSF firewall rules to allow OpenVPN server traffic

**Architectural Changes:**

| Change           | Before          | After                              |
| ---------------- | --------------- | ---------------------------------- |
| Shell            | `#!/bin/bash`   | `#!/bin/sh` (POSIX compatible)     |
| Package managers | apt-get only    | apt-get, dnf, yum (multi-distro)   |
| Config syntax    | Bash arrays     | POSIX strings                      |

**New Features:**

1. **7-Level Logging System** - Color-coded severity output (same as Docker script):
   - `verbose()` - Purple badge for verbose messages
   - `debug()` - Dark badge for debug (dev/dryrun only)
   - `info()` - Blue badge for informational
   - `ok()` - Green badge for success
   - `warn()` - Orange badge for warnings
   - `danger()` - Red badge for danger alerts
   - `error()` - Red badge for fatal errors

2. **Dryrun Mode** - `--dryrun` flag for safe testing without system changes

3. **Verbose Mode** - `--verbose` flag for detailed output

4. **Version Tracking** - App metadata with version 15.0.9

5. **Improved Configuration Variables:**
   - `ETH_ADAPTER` - Auto-detected or user-specified ethernet adapter
   - `IP_PUBLIC` - Auto-detected or user-specified public IP
   - `TUN_ADAPTER` - OpenVPN tunnel adapter (usually tun0)
   - `IP_POOL_LIST` - Space-separated list of VPN subnets

6. **Usage Modes:**
   - Automatic: Place in `/usr/local/include/csf/post.d/openvpn.sh`
   - Manual: `chmod +x openvpn.sh && sudo ./openvpn.sh`

**Backward Compatible:** Configuration variable names preserved; internal architecture modernized

### Shell Script POSIX Compliancy Refactoring (Commit [`b8cb8c005`](https://github.com/Aetherinox/csf-firewall/commit/b8cb8c005))

**Scope:** 5 shell scripts refactored for POSIX compliance
**Changes:** +102 / -441 lines (net reduction of 339 lines)

**Files Modified:**

- `src/global.sh` - Primary global functions library
- `src/csfpre.sh` - Pre-firewall hook script
- `src/csfpost.sh` - Post-firewall hook script
- `extras/scripts/docker.sh` - Docker integration
- `extras/scripts/openvpn.sh` - OpenVPN integration

**Key Changes:**

1. **Deprecated Bash-specific Functions** - Removed functions that relied on Bash-only features
2. **POSIX String Handling** - Replaced Bash arrays with POSIX-compatible string operations
3. **Portable Conditionals** - Changed `[[ ]]` to `[ ]` for POSIX compatibility
4. **Function Consolidation** - Merged redundant utility functions

**Impact:** Scripts now work across all POSIX-compliant shells (sh, dash, ash) in addition to Bash, improving compatibility with minimal Linux distributions and containers.

### 2026 Post-Rewrite Sync (releases 15.09, 15.10 and later — through 2026-06-16)

The fork rewrote its git history around February 2026 (see the note under Repository
State). After the rewrite, 131 genuinely new commits (111 touching `src/`) landed
between late January and 2026-06-16, spanning releases 15.09 (2026-02-23) and 15.10
(2026-02-28) plus post-15.10 development. Key changes:

**New Modules:**

- `ConfigServer/Sanitize.pm` ([`7a8a80e6b`](https://github.com/Aetherinox/csf-firewall/commit/7a8a80e6b)) - centralizes output sanitization; `strip_ansi` added in [`418efb136`](https://github.com/Aetherinox/csf-firewall/commit/418efb136), optional `chars` for `html_escape` in [`67e1210f7`](https://github.com/Aetherinox/csf-firewall/commit/67e1210f7)
- `ConfigServer/JSON.pm` ([`7f8a50ffb`](https://github.com/Aetherinox/csf-firewall/commit/7f8a50ffb)) - bundled JSON handling for migrated sponsor/license functions
- `ConfigServer/Perl/URI.pm` ([`417a7e91a`](https://github.com/Aetherinox/csf-firewall/commit/417a7e91a)) - bundles `URI::Escape`; external module requirement removed in [`fdb675e7b`](https://github.com/Aetherinox/csf-firewall/commit/fdb675e7b)
- `ConfigServer/Packages.pm` ([`858da7be3`](https://github.com/Aetherinox/csf-firewall/commit/858da7be3)) - package/dependency handling

**Security (XSS hardening wave, 2026-02-26 to 02-27):**

- [`c016aed1d`](https://github.com/Aetherinox/csf-firewall/commit/c016aed1d) - prevent XSS vulnerabilities; apply encode/escape
- [`c16215455`](https://github.com/Aetherinox/csf-firewall/commit/c16215455) - remove `innerHTML` potential XSS risk
- [`8a621bf31`](https://github.com/Aetherinox/csf-firewall/commit/8a621bf31) - remove `innerHTML` on scrollbar attachment
- [`0f26acd3c`](https://github.com/Aetherinox/csf-firewall/commit/0f26acd3c) - strip SGR escape sequences from exec command output

**ServerCheck / monitoring:**

- [`209005481`](https://github.com/Aetherinox/csf-firewall/commit/209005481) - auto-disable services from `Server Services Check` in web UI
- [`79ccaba65`](https://github.com/Aetherinox/csf-firewall/commit/79ccaba65) - Debian/Ubuntu detection in server distro check
- [`661a71ad4`](https://github.com/Aetherinox/csf-firewall/commit/661a71ad4) - new cPanel security check "Prevent user Nobody from sending email"
- [`acb4fa1ff`](https://github.com/Aetherinox/csf-firewall/commit/acb4fa1ff) - RBL status message lookup table with warning/info levels

**Configuration handling:**

- [`dcb125f37`](https://github.com/Aetherinox/csf-firewall/commit/dcb125f37) - preserve user comments in `csf.conf` across updates
- [`e7e37d3df`](https://github.com/Aetherinox/csf-firewall/commit/e7e37d3df) - dedicated `SECTION:` descriptions in config
- [`51f365ddb`](https://github.com/Aetherinox/csf-firewall/commit/51f365ddb) - `defaults.txt` + default values support in `ConfigServer::Config`
- [`a51a077ab`](https://github.com/Aetherinox/csf-firewall/commit/a51a077ab) - new setting `UI_WEBMIN_SHOW_BUTTON_CONFIG`

**UI / theming:**

- [`3b791a88e`](https://github.com/Aetherinox/csf-firewall/commit/3b791a88e) - dark theme integration; sprites added in [`4d6f4f098`](https://github.com/Aetherinox/csf-firewall/commit/4d6f4f098)
- [`cfd8d7123`](https://github.com/Aetherinox/csf-firewall/commit/cfd8d7123) - CyberPanel theme button synced with defined CSF theme
- [`247cc360c`](https://github.com/Aetherinox/csf-firewall/commit/247cc360c) - version-based cache busting for CSS/JS
- [`1754a2ec7`](https://github.com/Aetherinox/csf-firewall/commit/1754a2ec7) - condensed login retry indicator

**Fixes / misc:**

- [`ee1139396`](https://github.com/Aetherinox/csf-firewall/commit/ee1139396) - Dovecot 2.4 log format support
- [`e972771de`](https://github.com/Aetherinox/csf-firewall/commit/e972771de) - logfile responses for POP3 and IMAP
- [`6b3c62bc2`](https://github.com/Aetherinox/csf-firewall/commit/6b3c62bc2) - sanity check fix for `ST_ENABLE` (#114)
- [`e771ef9a5`](https://github.com/Aetherinox/csf-firewall/commit/e771ef9a5) - resolve `csf.c` compiler warnings for `main()`/`setenv()`
- [`da3f5c13e`](https://github.com/Aetherinox/csf-firewall/commit/da3f5c13e) - lfd logging refactor (current HEAD)

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
| `UI_CSP_ADVANCED_RULE`    | (default CSP string) | Custom CSP rule with template variable support; defaults to the full CSP directive string shown in the CSP analysis section | -     |
| `SPONSOR_ICON_ANIM`       | `"0"`   | Enable sponsor icon animation                    | -     |
| `SPONSOR_ICON_HIDE`       | `"0"`   | Hide sponsor icon in footer (renamed from `SPONSOR_HIDE_ICON`) | #72   |
| `SPONSOR_LICENSE`         | `""`    | License key (hides sponsor if set)               | -     |
| `SPONSOR_RELEASE_INSIDERS`| `"0"`   | Enable Insiders release channel                  | -     |
| `UI_WEBMIN_SHOW_BUTTON_CONFIG` | `"1"` | Show the config button in the Webmin module UI | -     |

---

## Commit Reference

Base sync commit: [`12c9f7c1f`](https://github.com/Aetherinox/csf-firewall/commit/12c9f7c1f) - Initial sync from official CSF v15.00

Key feature commits:

- [`12f9e1afc`](https://github.com/Aetherinox/csf-firewall/commit/12f9e1afc) - Theme selector (dark/light) - 21 files, +7,231 lines
- [`ae88914a3`](https://github.com/Aetherinox/csf-firewall/commit/ae88914a3) - Port listing command (`--listports/-lp`) - +59 lines
- [`5ccd44f17`](https://github.com/Aetherinox/csf-firewall/commit/5ccd44f17) - Port removal command (`--removeport/-rp`) - +118 lines
- [`93055acc3`](https://github.com/Aetherinox/csf-firewall/commit/93055acc3) - Port addition command (`--addport/-ap`) - +162 lines
- [`c876be73c`](https://github.com/Aetherinox/csf-firewall/commit/c876be73c) - License and insiders functions - +79 lines
- [`bd625f7f9`](https://github.com/Aetherinox/csf-firewall/commit/bd625f7f9) - Sponsor hide icon setting - 8 files
- [`f2a2e5206`](https://github.com/Aetherinox/csf-firewall/commit/f2a2e5206) - AbuseIPDB blocklist template - +16 lines
- [`036eccb34`](https://github.com/Aetherinox/csf-firewall/commit/036eccb34) - AlmaLinux/Rocky10/RedHat support - 7 files
- [`65bfcd75e`](https://github.com/Aetherinox/csf-firewall/commit/65bfcd75e) - Docker integration script rewrite - +1692/-960 lines
- [`aabd6bcc5`](https://github.com/Aetherinox/csf-firewall/commit/aabd6bcc5) - Docker command flags enhancement - +249/-164 lines
- [`d958f5f65`](https://github.com/Aetherinox/csf-firewall/commit/d958f5f65) - OpenVPN integration script rewrite - +1219/-243 lines

Security commits:

- [`edece43f6`](https://github.com/Aetherinox/csf-firewall/commit/edece43f6) - Harden sponsor functionality, eliminate client-side trust
- [`d85665f70`](https://github.com/Aetherinox/csf-firewall/commit/d85665f70) - Sanitize UI, use `textContent` instead of `innerHTML`
- [`ac61b07ca`](https://github.com/Aetherinox/csf-firewall/commit/ac61b07ca) - Default credential warning - 3 files, +424 lines
- [`37401ee0c`](https://github.com/Aetherinox/csf-firewall/commit/37401ee0c) - Content-Security-Policy headers - 7 files
- [`30405bcff`](https://github.com/Aetherinox/csf-firewall/commit/30405bcff) - Private network blocking - 7 files
- [`1037e4d8a`](https://github.com/Aetherinox/csf-firewall/commit/1037e4d8a) - Output sanitization functions - +78 lines
- [`77df09930`](https://github.com/Aetherinox/csf-firewall/commit/77df09930) - TTY detection for safe output - +7 lines

UI commits:

- [`1661d87e5`](https://github.com/Aetherinox/csf-firewall/commit/1661d87e5) - InterWorx iframe scrollbar fix
- [`015a69e65`](https://github.com/Aetherinox/csf-firewall/commit/015a69e65) - CyberPanel iframe scrollbar fix
- [`1f33294d8`](https://github.com/Aetherinox/csf-firewall/commit/1f33294d8) - CyberPanel footer padding fix
- [`c73b72a1e`](https://github.com/Aetherinox/csf-firewall/commit/c73b72a1e) - CSS class tags `value-restricted`, `value-disabled`
- [`522fcc616`](https://github.com/Aetherinox/csf-firewall/commit/522fcc616) - CyberPanel footer with theme selector
- [`69e172605`](https://github.com/Aetherinox/csf-firewall/commit/69e172605) - CWP new footer
- [`54a924443`](https://github.com/Aetherinox/csf-firewall/commit/54a924443) - DirectAdmin new footer
- [`8853f98f5`](https://github.com/Aetherinox/csf-firewall/commit/8853f98f5) - Comment formatting fix
- [`df6dc4651`](https://github.com/Aetherinox/csf-firewall/commit/df6dc4651) - Webmin settings button
- [`b47dd03a8`](https://github.com/Aetherinox/csf-firewall/commit/b47dd03a8) - Log refresh controls
- [`1498fa5f9`](https://github.com/Aetherinox/csf-firewall/commit/1498fa5f9) - Login failure notification
- [`aecdc1cfc`](https://github.com/Aetherinox/csf-firewall/commit/aecdc1cfc) - Sponsor button conditional display
- [`66402705a`](https://github.com/Aetherinox/csf-firewall/commit/66402705a) - Remove heart animation
- [`452ed724d`](https://github.com/Aetherinox/csf-firewall/commit/452ed724d) - GUI config editor formatting fix
- [`fd0bb6db4`](https://github.com/Aetherinox/csf-firewall/commit/fd0bb6db4) - Homepage buttons width fix
- [`43ce1c956`](https://github.com/Aetherinox/csf-firewall/commit/43ce1c956) - Interface header refactoring (lfd.pl)
- [`c95f9ae80`](https://github.com/Aetherinox/csf-firewall/commit/c95f9ae80) - Remove external dependency
- [`2afe04d9f`](https://github.com/Aetherinox/csf-firewall/commit/2afe04d9f) - Style conformity

2026 post-rewrite sync commits (15.09/15.10 and later):

- [`7a8a80e6b`](https://github.com/Aetherinox/csf-firewall/commit/7a8a80e6b) - New `ConfigServer/Sanitize.pm` module
- [`7f8a50ffb`](https://github.com/Aetherinox/csf-firewall/commit/7f8a50ffb) - New `ConfigServer/JSON.pm` module
- [`417a7e91a`](https://github.com/Aetherinox/csf-firewall/commit/417a7e91a) - Bundled `ConfigServer/Perl/URI.pm`
- [`858da7be3`](https://github.com/Aetherinox/csf-firewall/commit/858da7be3) - New `ConfigServer/Packages.pm` module
- [`c016aed1d`](https://github.com/Aetherinox/csf-firewall/commit/c016aed1d) - XSS prevention: encode/escape
- [`c16215455`](https://github.com/Aetherinox/csf-firewall/commit/c16215455) - Remove `innerHTML` XSS risk
- [`3b791a88e`](https://github.com/Aetherinox/csf-firewall/commit/3b791a88e) - Dark theme integration
- [`209005481`](https://github.com/Aetherinox/csf-firewall/commit/209005481) - Auto-disable services (Server Services Check)
- [`dcb125f37`](https://github.com/Aetherinox/csf-firewall/commit/dcb125f37) - Preserve user comments on csf updates
- [`ee1139396`](https://github.com/Aetherinox/csf-firewall/commit/ee1139396) - Dovecot 2.4 log support
- [`da3f5c13e`](https://github.com/Aetherinox/csf-firewall/commit/da3f5c13e) - lfd logging refactor (HEAD)

Refactoring commits:

- [`b8cb8c005`](https://github.com/Aetherinox/csf-firewall/commit/b8cb8c005) - Deprecate global bash functions; POSIX compliancy - 5 files, +102/-441 lines

---

Last updated: 2026-07-05
