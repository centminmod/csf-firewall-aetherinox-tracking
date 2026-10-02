# Aetherinox CSF Firewall Fork - Change Documentation

This document tracks all changes between the official CSF Firewall v15.00 (GPLv3) and the Aetherinox fork.

## Summary

| Category          | Count |
| ----------------- | ----- |
| Modified files    | 171   |
| New files         | 48    |
| Files removed     | 0     |
| Total differences | 219   |

**Fork Repository:** <https://github.com/Aetherinox/csf-firewall>

**Official CSF Repository:** <https://github.com/centminmod/configserver-scripts>

---

## Repository State (as of 2026-10-02)

| Repository | HEAD Commit | Date | Message |
|------------|-------------|------|---------|
| Official CSF | [`4793f7c`](https://github.com/centminmod/configserver-scripts/commit/4793f7c) | 2025-12-20 | update readme |
| Aetherinox Fork | [`0fcf47be1`](https://github.com/Aetherinox/csf-firewall/commit/0fcf47be1) | 2026-09-27 | feat(debug): add new module |

**Tracking source (2026-10):** fork HEAD is taken from `Aetherinox/csf-firewall`
(`upstream/main`) directly. The `centminmod/csf-firewall-aetherinox` mirror was still
at `da3f5c13e` on 2026-10-02, 48 commits behind upstream.

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
| Lines added       | 89,251     |
| Lines removed     | 34,483     |
| Net change        | +54,768    |
| Fork size (differing files only) | 13,684 KB  |
| Official size (differing files only) | 2,962 KB   |
| Size difference   | +10,722 KB |

Note: size figures sum only the modified and new files compared between trees
(full-tree byte totals are ~19,295 KB fork vs ~8,573 KB official).

### Most Changed Files (by commit count)

Ranking covers all 171 modified files (commit counts via `git log --follow` in the
fork repository). Ties are listed alphabetically.

| Rank | File                                  | Commits |
| ---- | ------------------------------------- | ------- |
| 1    | `ConfigServer/DisplayUI.pm`           | 56      |
| 2    | `csf.conf`                            | 41      |
| 3    | `csf.cwp.conf`                        | 40      |
| 4    | `csf.cyberpanel.conf`                 | 40      |
| 5    | `csf.directadmin.conf`                | 40      |
| 6    | `csf.generic.conf`                    | 40      |
| 7    | `csf.interworx.conf`                  | 40      |
| 8    | `csf.vesta.conf`                      | 40      |
| 9    | `csf/configserver.css`                | 40      |
| 10   | `da/images/configserver.css`          | 33      |

---

## New Files (48 files)

Files that exist only in the Aetherinox fork.

### New Perl Modules

| File | Description | Initial Commit |
|------|-------------|----------------|
| `csf-firewall-aetherinox/src/ConfigServer/JSON.pm` | Bundled JSON encode/decode module (used by sponsor/license functions) | [`7f8a50ffb`](https://github.com/Aetherinox/csf-firewall/commit/7f8a50ffb) |
| `csf-firewall-aetherinox/src/ConfigServer/Packages.pm` | Package/dependency handling module | [`858da7be3`](https://github.com/Aetherinox/csf-firewall/commit/858da7be3) |
| `csf-firewall-aetherinox/src/ConfigServer/Perl/URI.pm` | Bundled `URI::Escape` (drops external module requirement) | [`417a7e91a`](https://github.com/Aetherinox/csf-firewall/commit/417a7e91a) |
| `csf-firewall-aetherinox/src/ConfigServer/Sanitize.pm` | Output sanitization helpers (`html_escape`, `strip_ansi`) | [`7a8a80e6b`](https://github.com/Aetherinox/csf-firewall/commit/7a8a80e6b) |
| `csf-firewall-aetherinox/src/ConfigServer/Debug.pm` | Leveled debug helper: `log()` writes to stderr, `getopts()`/`dump()` format text; level from `ENV{DEBUG}` (0-5); not yet imported by any module | [`0fcf47be1`](https://github.com/Aetherinox/csf-firewall/commit/0fcf47be1) |
| `csf-firewall-aetherinox/src/ConfigServer/Secrets.pm` | Staged stub for secret redaction (package + `use` lines only, no subs yet); lazily required by `Debug.pm` | [`e789a9d76`](https://github.com/Aetherinox/csf-firewall/commit/e789a9d76) |

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
| `csf-firewall-aetherinox/src/defaults.txt` | Default values reference, read only by `ConfigServer::Config::getdefault()` (no callers yet; not merged into `loadconfig()`) | [`51f365ddb`](https://github.com/Aetherinox/csf-firewall/commit/51f365ddb) |
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
| [`a23ffc8cf`](https://github.com/Aetherinox/csf-firewall/commit/a23ffc8cf) | feat(lfd): add option `LFD_PROCESS_BIND` to restrict PID ownership checks to parent process |
| [`c57aa3a2f`](https://github.com/Aetherinox/csf-firewall/commit/c57aa3a2f) | fix(syntax): lfd startup syntax error                                                    |
| [`a94ca865a`](https://github.com/Aetherinox/csf-firewall/commit/a94ca865a) | chore(cfg): update `LF_INTEGRITY` minimum threshold to 120s                              |
| [`43ce1c956`](https://github.com/Aetherinox/csf-firewall/commit/43ce1c956) | refactor(generic): update interface header                                               |
| [`ac61b07ca`](https://github.com/Aetherinox/csf-firewall/commit/ac61b07ca) | feat(csf): add warning to console output when using default web ui username and password |

**Key Changes:**

- Security warning for default credentials
- Interface header refactoring with structured HTML layout (header-left/header-right divs)
- New `LFD_PROCESS_BIND` option: when `1`, only the master lfd process checks the PID
  file and performs a full shutdown; child processes log and exit individually
- `c57aa3a2f` fixes a stray `s` line that made `lfd.pl` at `da3f5c13e` fail to compile
  ("Substitution pattern not terminated"), adds missing semicolons and reformats `sub portscans`
- `LF_INTEGRITY` floor moved into `$MIN_INTEGRITY_INTERVAL = 120` (values below 120
  still revert to 300, as in official)

### csf.conf (Main Configuration)

**Path:** `csf-firewall-aetherinox/src/csf.conf`

**Commit History (Recent):**

| Commit      | Description                                                                               |
| ----------- | ----------------------------------------------------------------------------------------- |
| [`bb5235f48`](https://github.com/Aetherinox/csf-firewall/commit/bb5235f48) | chore(csf): update default settings and descriptions                                      |
| [`5d4d9cd6d`](https://github.com/Aetherinox/csf-firewall/commit/5d4d9cd6d) | chore(cfg): update `MESSENGER` config notes                                               |
| [`a23ffc8cf`](https://github.com/Aetherinox/csf-firewall/commit/a23ffc8cf) | feat(lfd): add option `LFD_PROCESS_BIND` to restrict PID ownership checks to parent process |
| [`a95b63d62`](https://github.com/Aetherinox/csf-firewall/commit/a95b63d62) | chore(cfg): update `LOGSCANNER` with globs warning                                        |
| [`a94ca865a`](https://github.com/Aetherinox/csf-firewall/commit/a94ca865a) | chore(cfg): update `LF_INTEGRITY` minimum threshold to 120s                               |
| [`4f680e295`](https://github.com/Aetherinox/csf-firewall/commit/4f680e295) | chore(cfg): update setting `LF_DIRWATCH`                                                  |
| [`e4e1f4237`](https://github.com/Aetherinox/csf-firewall/commit/e4e1f4237) | chore(cfg): update setting `LF_EXPLOIT`                                                   |
| [`c9336994a`](https://github.com/Aetherinox/csf-firewall/commit/c9336994a) | chore(cfg): update setting `CC_LOOKUPS`                                                   |
| [`3aabe3966`](https://github.com/Aetherinox/csf-firewall/commit/3aabe3966) | chore(cfg): update setting `CC_IGNORE`                                                    |
| [`dd5b5d777`](https://github.com/Aetherinox/csf-firewall/commit/dd5b5d777) | chore(cfg): update setting `PT_LIMIT`                                                     |
| [`d2b6358d0`](https://github.com/Aetherinox/csf-firewall/commit/d2b6358d0) | chore(cfg): separate setting `GLOBAL_*` with proper description                           |
| [`7bd25d444`](https://github.com/Aetherinox/csf-firewall/commit/7bd25d444) | chore(cfg): separate setting `LF_GLOBAL` with proper description                          |
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
| `UI_WEBMIN_SHOW_BUTTON_CONFIG` | Show config button in Webmin module ([`a51a077ab`](https://github.com/Aetherinox/csf-firewall/commit/a51a077ab)) | -     |
| `LFD_PROCESS_BIND`        | Restrict PID-file checks and full shutdown to the lfd parent process ([`a23ffc8cf`](https://github.com/Aetherinox/csf-firewall/commit/a23ffc8cf)) | -     |

The 2026-08/09 `chore(cfg)` commits only rewrite comments and descriptions
(`LF_GLOBAL`, `GLOBAL_*`, `PT_LIMIT`, `CC_IGNORE`, `CC_LOOKUPS`, `LF_EXPLOIT`,
`LF_DIRWATCH`, `LF_INTEGRITY`, `LOGSCANNER`, `MESSENGER*`); no existing default value
changed.

---

## Modified Files - ConfigServer Modules (24 files)

All Perl modules in `csf-firewall-aetherinox/src/ConfigServer/` directory.

### DisplayUI.pm (Web Interface)

**Commit History:**

| Commit      | Description                                                                                |
| ----------- | ------------------------------------------------------------------------------------------ |
| [`f379f0b63`](https://github.com/Aetherinox/csf-firewall/commit/f379f0b63) | Fix(#123): stray apostrophe in `<b>` tag generates invalid HTML                            |
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
- Config editor select line: `<b'>$start</b>` corrected to `<b>$start</b>` (#123)

### DisplayResellerUI.pm

**Changes:** Reseller UI modifications paralleling DisplayUI.pm changes

### URLGet.pm (HTTP Fetch Hardening, 2026-08)

**Commit History:**

| Commit      | Description                                                                              |
| ----------- | ---------------------------------------------------------------------------------------- |
| [`975fad924`](https://github.com/Aetherinox/csf-firewall/commit/975fad924) | refactor(urlget): rename URLGet method and timeout variables                             |
| [`049834e94`](https://github.com/Aetherinox/csf-firewall/commit/049834e94) | chore(urlget): limit max url length passed to urlget package                             |
| [`b0e295a28`](https://github.com/Aetherinox/csf-firewall/commit/b0e295a28) | fix(urlget): reject control chars; block crlf/nul injection                              |
| [`bfe81e5e4`](https://github.com/Aetherinox/csf-firewall/commit/bfe81e5e4) | fix(urlget): use `cmd_label` instead of hard string label for utilities                  |
| [`edb5bd01f`](https://github.com/Aetherinox/csf-firewall/commit/edb5bd01f) | fix(urlget): prevent command injection in curl/wget fallback; build argv instead of shell string |
| [`1d23805ce`](https://github.com/Aetherinox/csf-firewall/commit/1d23805ce) | fix(urlget): correct completed request logging order                                     |
| [`0ac5932f8`](https://github.com/Aetherinox/csf-firewall/commit/0ac5932f8) | fix(urlget): redact sensitive parameters from requests                                   |
| [`57b210322`](https://github.com/Aetherinox/csf-firewall/commit/57b210322) | fix(urlget): remove duplicate request                                                    |

**Key Changes:**

- curl/wget fallback (`_method_curlwget`) now runs an argv list through `open3`
  instead of a `/bin/sh` command string, which removes shell command injection
- `urlget()` rejects control characters (CR/LF/NUL), non-`http(s)://` schemes and
  URLs longer than 2,048 characters (`$GET_URL_LEN_MAX`)
- New `_url_sanitize()` redacts `key`, `license`, `token`, `password` and similar
  query values in debug logs and returned error strings
- Every `urlget()` call previously issued the request twice; the duplicate is removed
- Timeouts moved into `$GET_TIMEOUT_CONNECT` (300s) and `$GET_TIMEOUT_ALARM` (600s);
  HTTP::Tiny alarm drops from 1200s to 600s, LWP alarm rises from 300s to 600s and the
  LWP client timeout from 30s to 300s
- Redaction gap: the `DEBUG` log line in `_with_alarm_timeout` still prints the raw `$err`
  (the returned error string is sanitized)

### Messenger.pm (2026-08 to 2026-09)

**Commit History:**

| Commit      | Description                                                                              |
| ----------- | ---------------------------------------------------------------------------------------- |
| [`8464e0081`](https://github.com/Aetherinox/csf-firewall/commit/8464e0081) | chore: push pending commits (Messenger.pm reformat, extra debug logging)                 |
| [`0b9509a82`](https://github.com/Aetherinox/csf-firewall/commit/0b9509a82) | chore(messenger): define packages                                                        |
| [`33682f541`](https://github.com/Aetherinox/csf-firewall/commit/33682f541) | fix(messenger): original code parentheses bug                                            |
| [`7946ea17e`](https://github.com/Aetherinox/csf-firewall/commit/7946ea17e) | refactor(messenger): housekeeping                                                        |
| [`f13f3aa96`](https://github.com/Aetherinox/csf-firewall/commit/f13f3aa96) | fix(messenger): write recaptcha.php with `0600` permissions                              |
| [`f9168fa9e`](https://github.com/Aetherinox/csf-firewall/commit/f9168fa9e) | fix(messenger): prevent running with root uid/gid                                        |

**Key Changes:**

- `messenger()`, `messengerv2()` and `messengerv3()` all refuse to run when
  `MESSENGER_USER` resolves to uid/gid 0 or is invalid (official v2/v3 had no check)
- `recaptcha.php` (holds the reCAPTCHA secret) is written with mode `600` instead of `644`
- `scalar(keys %sslcerts < 1)` rewritten as `!keys %sslcerts` in v1 (equivalent in Perl, since
  `keys` binds tighter than `<`; v2/v3 keep the old form); the error now names
  `MESSENGER_HTTPS_CONF`
- Added `PACKAGE_NAME` / `SUB_MESSENGER_V*` constants and `DEBUG`-gated logging

### CheckIP.pm

**Commit History:**

| Commit      | Description                                                                              |
| ----------- | ---------------------------------------------------------------------------------------- |
| [`378f639f1`](https://github.com/Aetherinox/csf-firewall/commit/378f639f1) | feat: add updated checkip module                                                         |
| [`03e635d44`](https://github.com/Aetherinox/csf-firewall/commit/03e635d44) | fix(checkip): reject IPv4 and IPv6 /0 CIDR prefixes                                      |

**Key Changes:**

- `checkip()` / `cccheckip()` used `if ($cidr)`, so a `/0` prefix (string `"0"` is
  false in Perl) skipped the range check and was accepted; now `/0` is rejected for
  IPv4 and IPv6
- IPv6 loopback test changed from numeric `$ip == 1` to string `$ip eq "1"`, so stripped
  addresses that merely start with `1` are no longer treated as loopback
- Module reformatted, `$VERSION` 1.03 → 15.11, new non-exported `tests_checkip()`
  self-test helper; exported API (`checkip`, `cccheckip`) unchanged

### Logger.pm, Config.pm, GetIPs.pm, Sendmail.pm (2026-08 to 2026-09)

**Commit History:**

| Commit      | Description                                                                              |
| ----------- | ---------------------------------------------------------------------------------------- |
| [`2c6192684`](https://github.com/Aetherinox/csf-firewall/commit/2c6192684) | fix(logger): detect globally executed code not specifically in subroutine                |
| [`88b12088e`](https://github.com/Aetherinox/csf-firewall/commit/88b12088e) | feat(logger): add calling sub name                                                       |
| [`389ec3588`](https://github.com/Aetherinox/csf-firewall/commit/389ec3588) | chore(sendmail): full sendmail message migrated to `DEBUG:2`                             |
| [`beac44664`](https://github.com/Aetherinox/csf-firewall/commit/beac44664) | chore: housekeeping (`Config.pm` `$VERSION` 15.11, comment fixes)                        |
| [`822c39413`](https://github.com/Aetherinox/csf-firewall/commit/822c39413) | style(config): update whitespace formatting                                              |
| [`3c061d50f`](https://github.com/Aetherinox/csf-firewall/commit/3c061d50f) | feat(config): add sub `getsingle`                                                        |
| [`b3f100e22`](https://github.com/Aetherinox/csf-firewall/commit/b3f100e22) | refactor(logger): modernize logging, add lazy config loading                             |
| [`560c20ba5`](https://github.com/Aetherinox/csf-firewall/commit/560c20ba5) | feat(logger): add leveled debug logging helper                                           |
| [`371ff5eea`](https://github.com/Aetherinox/csf-firewall/commit/371ff5eea) | chore(getips): re-write module                                                           |
| [`5390afc2d`](https://github.com/Aetherinox/csf-firewall/commit/5390afc2d) | chore: import `ConfigServer::Logger` in module `Sendmail`                                |

**Key Changes:**

- `Logger::logfile()` rewritten: forms `logfile(message)`, `logfile(status, message)` and
  `logfile(type, status, message)` with types `normal`, `root`, `all`, `DEBUG:0`-`DEBUG:5`;
  named or numeric status (FAIL/OK/WARN/ABORT/INFO), a separate root log `lfd-root.log`,
  caller tag `file:line->sub()`, lazy config/syslog loading, and a result hashref for
  written or suppressed lines (was `undef`)
- `logfile()` gates `DEBUG:1`-`DEBUG:5` lines against `csf.conf` `DEBUG` (official
  `lfd.pl` already compared `DEBUG >= n`); the full failed Sendmail message is now
  logged only at `DEBUG >= 2`
- New `ConfigServer::Config->getsingle($item)` reads one `csf.conf` key without
  running `loadconfig()` validation (used by `CheckIP.pm`)
- `GetIPs.pm` rewritten: `getips()` renamed to `resolve()`, `hex2ip`/`ip2hex`/`ipv4in6`
  moved in, Exporter removed (see Known Issues under Detailed Change Analysis)

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
| `CheckIP.pm`     | See CheckIP.pm section above  |
| `CloudFlare.pm`  | Header updates, formatting    |
| `Config.pm`      | Config parsing; `getsingle()` (see Logger.pm section) |
| `GetEthDev.pm`   | Network device detection      |
| `GetIPs.pm`      | Rewritten (see Logger.pm section, Known Issues) |
| `KillSSH.pm`     | SSH rate limiting             |
| `Logger.pm`      | See Logger.pm section above   |
| `LookUpIP.pm`    | IP lookup functionality       |
| `Messenger.pm`   | See Messenger.pm section above |
| `Ports.pm`       | Port management               |
| `RBLCheck.pm`    | RBL checking                  |
| `RBLLookup.pm`   | RBL lookup                    |
| `RegexMain.pm`   | Regex pattern matching        |
| `Sanity.pm`      | System validation             |
| `Sendmail.pm`    | Failed-message logging moved to `DEBUG:2` |
| `ServerCheck.pm` | Server monitoring             |
| `ServerStats.pm` | Statistics collection         |
| `Service.pm`     | Service management            |
| `Slurp.pm`       | File reading                  |
| `URLGet.pm`      | See URLGet.pm section above   |
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

**Key-level differences vs official platform configs:**

| Change | Files | Commit |
| ------ | ----- | ------ |
| `LFD_PROCESS_BIND = "0"` added | all 7 `csf*.conf` | [`a23ffc8cf`](https://github.com/Aetherinox/csf-firewall/commit/a23ffc8cf) |
| `MESSENGERV2 = "0"` uncommented (official ships it as `#MESSENGERV2 = "0"`) | 6 platform confs (already active in `csf.conf`) | [`bb5235f48`](https://github.com/Aetherinox/csf-firewall/commit/bb5235f48) |
| `LF_APACHE_401_PERM` line dropped during a comment reformat | `csf.cwp.conf`, `csf.cyberpanel.conf`, `csf.interworx.conf` | [`353bfe2c0`](https://github.com/Aetherinox/csf-firewall/commit/353bfe2c0) |
| `LF_APACHE_401_PERM` line dropped during a comment reformat | `csf.vesta.conf` | [`b3a24e6fd`](https://github.com/Aetherinox/csf-firewall/commit/b3a24e6fd) |
| `LF_APACHE_404_PERM` line dropped during a comment reformat | `csf.generic.conf` | [`353bfe2c0`](https://github.com/Aetherinox/csf-firewall/commit/353bfe2c0) |
| `RT_POPRELAY_ALERT` / `_LIMIT` / `_BLOCK` present (absent from official) | `csf.directadmin.conf` | [`43a2a7d6e`](https://github.com/Aetherinox/csf-firewall/commit/43a2a7d6e) |

The dropped `LF_APACHE_40x_PERM` keys are still read by `lfd.pl` (`disable401`/`disable404`).
`defaults.txt` lists both at `3600`, but nothing merges it into the loaded config
(`getdefault()` has no callers), so on these platforms the key is undefined, `lfd.pl`
sets `$perm = 1`, and `LF_APACHE_401`/`LF_APACHE_404` blocks become permanent instead of
3600-second temporary blocks. Impact is limited to admins who enable those features
(both default to `"0"`). Both removals landed on 2025-10-07 in config-reformat commits
(`353bfe2c0` is titled "chore(ssl): update ssl cert and key for web interface"), so they
look accidental.

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
| `install.*.sh` (7 files)    | Also copy `messenger/*.html` on install/update ([`d82b1fc68`](https://github.com/Aetherinox/csf-firewall/commit/d82b1fc68)) |

### Messenger Web Files

These three files matched official CSF through `da3f5c13e` (2026-06-16) and diverged
in September 2026:

| File | Changes | Commits |
| ---- | ------- | ------- |
| `messenger/index.php` | `HTTP_ACCEPT_LANGUAGE` lowercased and whitelisted to `^[a-z]{2}$`; language and `recaptcha.php` loaded via `dirname(__DIR__)` with `is_file()` checks | [`1e7f9ada3`](https://github.com/Aetherinox/csf-firewall/commit/1e7f9ada3) |
| `messenger/index.html` | Logo swapped from PNG to SVG data URI (also in `index.php` and `index.recaptcha.php`) | [`1e7f9ada3`](https://github.com/Aetherinox/csf-firewall/commit/1e7f9ada3) |
| `messenger/index.recaptcha.php` | cURL connect/total timeouts; JSON response validation (`success`, `hostname`); `htmlspecialchars()` on reflected `REQUEST_URI` and hostnames (reflected XSS fix); unblock-file write checked and logged (the page still shows success if the write fails); error logging | [`904d9a65f`](https://github.com/Aetherinox/csf-firewall/commit/904d9a65f), [`568f9a309`](https://github.com/Aetherinox/csf-firewall/commit/568f9a309) |

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
| URLGet command injection fix | curl/wget fallback runs an argv list, not a shell string ([`edb5bd01f`](https://github.com/Aetherinox/csf-firewall/commit/edb5bd01f)) |
| URLGet input validation      | Reject control chars, non-HTTP(S) schemes, URLs > 2,048 chars ([`b0e295a28`](https://github.com/Aetherinox/csf-firewall/commit/b0e295a28), [`049834e94`](https://github.com/Aetherinox/csf-firewall/commit/049834e94)) |
| URLGet secret redaction      | License/API key/token values redacted from logs and errors ([`0ac5932f8`](https://github.com/Aetherinox/csf-firewall/commit/0ac5932f8)) |
| Messenger privilege check    | Refuse to run Messenger v1/v2/v3 as uid/gid 0 ([`f9168fa9e`](https://github.com/Aetherinox/csf-firewall/commit/f9168fa9e)) |
| reCAPTCHA secret permissions | `recaptcha.php` written `0600` instead of `0644` ([`f13f3aa96`](https://github.com/Aetherinox/csf-firewall/commit/f13f3aa96)) |
| reCAPTCHA page hardening     | Escape reflected `REQUEST_URI`/hostnames, validate Google response ([`904d9a65f`](https://github.com/Aetherinox/csf-firewall/commit/904d9a65f)) |
| Messenger language whitelist | `index.php` accepts only `^[a-z]{2}$` language codes ([`1e7f9ada3`](https://github.com/Aetherinox/csf-firewall/commit/1e7f9ada3)) |
| `/0` CIDR rejection          | `checkip()`/`cccheckip()` reject IPv4/IPv6 `/0` prefixes ([`03e635d44`](https://github.com/Aetherinox/csf-firewall/commit/03e635d44)) |

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
| lfd startup syntax (missing semicolons)  | [`c57aa3a2f`](https://github.com/Aetherinox/csf-firewall/commit/c57aa3a2f) |
| URLGet duplicate request per call        | [`57b210322`](https://github.com/Aetherinox/csf-firewall/commit/57b210322) |
| URLGet completed-request log order       | [`1d23805ce`](https://github.com/Aetherinox/csf-firewall/commit/1d23805ce) |
| Invalid `<b'>` HTML in config editor (#123) | [`f379f0b63`](https://github.com/Aetherinox/csf-firewall/commit/f379f0b63) |

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
- [`da3f5c13e`](https://github.com/Aetherinox/csf-firewall/commit/da3f5c13e) - lfd logging refactor (HEAD as of 2026-07-05)

### 2026-Q3 Sync (post-15.10, v15.11 prep — through 2026-09-27)

48 commits landed between `da3f5c13e` (2026-06-16) and `0fcf47be1` (2026-09-27);
46 touch `src/` (28 files, +5,947/-1,801 lines net, per `git diff --shortstat`). The other two are CI-only
([`de1aedf67`](https://github.com/Aetherinox/csf-firewall/commit/de1aedf67) release
workflow prep for v15.11, [`96e5daf87`](https://github.com/Aetherinox/csf-firewall/commit/96e5daf87)
`renovate.json`). No new release tag yet; 15.10 is still the latest.

**New option: `LFD_PROCESS_BIND`** ([`a23ffc8cf`](https://github.com/Aetherinox/csf-firewall/commit/a23ffc8cf))

- Default `"0"` (previous behaviour): any lfd process may validate the PID file and
  perform a full shutdown on error.
- `"1"` (any true value): only the master process (`$$ == $masterpid`) runs the PID-file/inode check;
  in `sub shutdown`, a child logs `[SHUTDOWN] Child Process: ...` and exits 0 without
  removing the PID file or stopping the daemon.
- Not listed in `defaults.txt`; `lfd.pl` treats an undefined value as `0`.

**Logging rework** ([`560c20ba5`](https://github.com/Aetherinox/csf-firewall/commit/560c20ba5),
[`b3f100e22`](https://github.com/Aetherinox/csf-firewall/commit/b3f100e22),
[`88b12088e`](https://github.com/Aetherinox/csf-firewall/commit/88b12088e),
[`2c6192684`](https://github.com/Aetherinox/csf-firewall/commit/2c6192684))

- `logfile(message)`, `logfile(status, message)` or `logfile(type, status, message)`;
  types `normal`, `root`, `all`, `DEBUG:0`-`DEBUG:5`.
- `DEBUG:1`-`DEBUG:5` lines are written only when `csf.conf` `DEBUG` is at or above
  that level; `DEBUG:0` is always written.
- Root-only messages go to `lfd-root.log` without loading the CSF config.
- Each line carries a `file:line->sub()` source tag (`::global` outside a sub).

**New modules:**

- `ConfigServer/Debug.pm` ([`0fcf47be1`](https://github.com/Aetherinox/csf-firewall/commit/0fcf47be1),
  788 lines): debug helper (`log()` to stderr; `getopts()`/`dump()` format text) driven by the
  `DEBUG` environment variable, not `csf.conf`. Nothing imports it yet.
- `ConfigServer/Secrets.pm` ([`e789a9d76`](https://github.com/Aetherinox/csf-firewall/commit/e789a9d76),
  71 lines): staged stub with no subs and no trailing `1;`, so `require` fails with
  "did not return a true value". `Debug.pm` lazily requires it (levels 1-4) and then calls
  `redact_obj_log`/`redact_obj_field`, which do not exist yet.

**Security hardening:** URLGet argv execution, URL validation and secret redaction;
Messenger root-uid refusal and `0600` secret file; reCAPTCHA page output escaping;
`index.php` language whitelist; `/0` CIDR rejection. See the URLGet.pm, Messenger.pm,
CheckIP.pm and Messenger Web Files sections above.

**Known issues (static analysis plus minimal Perl reproductions; not run on a live server):**

| Issue | Location | Introduced |
| ----- | -------- | ---------- |
| `ServerCheck.pm` has not compiled on `main` since `209005481` (2026-03-01); the 15.10 release copy compiles. At HEAD, `332a26cde` removed the `sub report {` header, leaving the report body at file scope and an unmatched `}` ("Unmatched right curly bracket"). `csf.pl` and `DisplayUI.pm` both `use ConfigServer::ServerCheck`, so on current `main` the `csf` command and the web UI fail to load, and `ConfigServer::ServerCheck::report()` no longer exists for its two callers. Verified by compiling each revision with stub dependencies. | `ConfigServer/ServerCheck.pm:194`; callers `csf.pl:43`, `csf.pl:6321`, `ConfigServer/DisplayUI.pm:44`, `ConfigServer/DisplayUI.pm:1139` | [`209005481`](https://github.com/Aetherinox/csf-firewall/commit/209005481), [`332a26cde`](https://github.com/Aetherinox/csf-firewall/commit/332a26cde) |
| `GetIPs.pm` no longer defines `getips()` or uses Exporter, but callers still `use ConfigServer::GetIPs qw(getips)`. The import compiles silently and the call dies with `Undefined subroutine`. In Messenger v1 the call sits inside the child's `eval`, so a reCAPTCHA unblock request fails silently (Google returns a hostname). The `whmcheck` call (cPanel, hostname nameservers) will die the same way once `ServerCheck.pm` compiles again. | `ConfigServer/Messenger.pm:535` (`messenger`), `ConfigServer/ServerCheck.pm:1365` (`whmcheck`); unused import in `RBLCheck.pm:37` | [`371ff5eea`](https://github.com/Aetherinox/csf-firewall/commit/371ff5eea) |
| Same failure mode, older: `ServerCheck.pm` does `use ConfigServer::Sanity qw(sanity)` and calls `sanity()` for each `csf.conf` setting in `firewallcheck`, but `Sanity.pm` no longer exports it (official does). Once `ServerCheck.pm` compiles again, every Server Security Check report will die here. | `ConfigServer/ServerCheck.pm:37`, `ConfigServer/ServerCheck.pm:466` | [`3659719ca`](https://github.com/Aetherinox/csf-firewall/commit/3659719ca) (2026-03-05) |
| Language hardening from `index.php` was not applied to `index.recaptcha.php`, which still uses `substr(HTTP_ACCEPT_LANGUAGE,0,2)` with `file_exists()`. It still sets `CURLOPT_SSL_VERIFYPEER` to `false` for the Google verify call. | `messenger/index.recaptcha.php` | pre-existing (official) |
| `Debug.pm` redaction path (`DEBUG` levels 1-4) requires `Secrets.pm`, which fails to load (no `1;`) and does not define `redact_obj_log`/`redact_obj_field` yet; nothing imports `Debug.pm` yet | `ConfigServer/Debug.pm`, `ConfigServer/Secrets.pm` | [`0fcf47be1`](https://github.com/Aetherinox/csf-firewall/commit/0fcf47be1), [`e789a9d76`](https://github.com/Aetherinox/csf-firewall/commit/e789a9d76) |

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
| `LFD_PROCESS_BIND`        | `"0"`   | `1` = only the lfd parent process may check the PID file and stop the daemon; children log and exit individually | -     |

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
- [`da3f5c13e`](https://github.com/Aetherinox/csf-firewall/commit/da3f5c13e) - lfd logging refactor (HEAD as of 2026-07-05)

2026-Q3 sync commits (post-15.10, v15.11 prep):

- [`edb5bd01f`](https://github.com/Aetherinox/csf-firewall/commit/edb5bd01f) - URLGet: argv execution, removes shell command injection
- [`b0e295a28`](https://github.com/Aetherinox/csf-firewall/commit/b0e295a28) - URLGet: reject control chars and non-HTTP(S) URLs
- [`0ac5932f8`](https://github.com/Aetherinox/csf-firewall/commit/0ac5932f8) - URLGet: redact secrets in logs/errors
- [`57b210322`](https://github.com/Aetherinox/csf-firewall/commit/57b210322) - URLGet: remove duplicate request
- [`f9168fa9e`](https://github.com/Aetherinox/csf-firewall/commit/f9168fa9e) - Messenger: refuse root uid/gid
- [`f13f3aa96`](https://github.com/Aetherinox/csf-firewall/commit/f13f3aa96) - Messenger: `recaptcha.php` mode 0600
- [`904d9a65f`](https://github.com/Aetherinox/csf-firewall/commit/904d9a65f) - reCAPTCHA page hardening (output escaping, response validation)
- [`1e7f9ada3`](https://github.com/Aetherinox/csf-firewall/commit/1e7f9ada3) - Messenger `index.php` language whitelist
- [`03e635d44`](https://github.com/Aetherinox/csf-firewall/commit/03e635d44) - CheckIP: reject `/0` prefixes
- [`378f639f1`](https://github.com/Aetherinox/csf-firewall/commit/378f639f1) - CheckIP module update (v15.11)
- [`a23ffc8cf`](https://github.com/Aetherinox/csf-firewall/commit/a23ffc8cf) - New option `LFD_PROCESS_BIND`
- [`b3f100e22`](https://github.com/Aetherinox/csf-firewall/commit/b3f100e22) - Logger rewrite (types, DEBUG levels, root log)
- [`3c061d50f`](https://github.com/Aetherinox/csf-firewall/commit/3c061d50f) - Config: new `getsingle()`
- [`371ff5eea`](https://github.com/Aetherinox/csf-firewall/commit/371ff5eea) - GetIPs rewrite (`getips` → `resolve`; see Known Issues)
- [`e789a9d76`](https://github.com/Aetherinox/csf-firewall/commit/e789a9d76) - New `ConfigServer/Secrets.pm` stub
- [`0fcf47be1`](https://github.com/Aetherinox/csf-firewall/commit/0fcf47be1) - New `ConfigServer/Debug.pm` module (HEAD)

Refactoring commits:

- [`b8cb8c005`](https://github.com/Aetherinox/csf-firewall/commit/b8cb8c005) - Deprecate global bash functions; POSIX compliancy - 5 files, +102/-441 lines

---

Last updated: 2026-10-02
