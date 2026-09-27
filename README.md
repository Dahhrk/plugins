# Cursor plugins

Official Cursor plugins for popular developer tools, frameworks, and SaaS products. Each plugin is a standalone directory at the repository root with its own `.cursor-plugin/plugin.json` manifest.

## Plugins

| `name` | Plugin | Author | Category | `description` (from marketplace) |
|:-------|:-------|:-------|:---------|:-------------------------------------|
| `teaching` | [Teaching](teaching/) | Cursor | Utilities | Skill mapping, practice plans, and learning retrospectives. |
| `continual-learning` | [Continual Learning](continual-learning/) | Cursor | Developer Tools | Incremental transcript-driven memory updates for AGENTS.md using high-signal bullet points only. |
| `cursor-team-kit` | [Cursor Team Kit](cursor-team-kit/) | Cursor | Developer Tools | Internal team workflows for CI, code review, shipping, local automation, and verification. |
| `thermos` | [Thermos](thermos/) | Cursor | Developer Tools | Thermo-nuclear branch review: deep security/correctness audits, harsh code-quality rubrics, parallel subagents, thermos orchestration, and optional merge-ready PR flows. |
| `create-plugin` | [Create Plugin](create-plugin/) | Cursor | Developer Tools | Scaffold and validate new agent plugins. |
| `ralph-loop` | [Ralph Loop](ralph-loop/) | Cursor | Developer Tools | Iterative self-referential AI loops using the Ralph Wiggum technique. |
| `agent-compatibility` | [Agent Compatibility](agent-compatibility/) | Cursor | Developer Tools | CLI-backed repo compatibility scans plus agents that audit startup, validation, and docs against reality. |
| `cli-for-agent` | [CLI for Agents](cli-for-agent/) | Cursor | Developer Tools | Patterns for designing CLIs that coding agents can run reliably: flags, help with examples, pipelines, errors, idempotency, dry-run. |
| `pr-review-canvas` | [PR Review Canvas](pr-review-canvas/) | Cursor | Developer Tools | Render PR diffs as review canvases grouped by importance. |
| `docs-canvas` | [Docs Canvas](docs-canvas/) | Cursor | Developer Tools | Render documentation as a navigable canvas. |
| `cursor-sdk` | [Cursor SDK](cursor-sdk/) | Cursor | Developer Tools | Build apps, scripts, and automations with the TypeScript SDK. |
| `orchestrate` | [Orchestrate](orchestrate/) | Cursor | Developer Tools | Fan large tasks out across parallel cloud agents with planners, workers, verifiers, and structured handoffs. |
| `pstack` | [pstack](pstack/) | Lauren Tan | Developer Tools | if you want to go fast, go deep first. pstack helps you write less, but higher quality code. rigorous agent workflows you can parallelize with confidence. |
| `lua-kit` | [Lua Kit](lua-kit/) | Dahhrk | Developer Tools | GMod Lua bar: poteto EXIT, PSR Lua ch.4 (formatter/linter, scope, table-shape, host, version/host), rg+hotpath+luacheck+glualint required, Facepunch extras. |
| `typescript-kit` | [Typescript Kit](typescript-kit/) | Dahhrk | Developer Tools | TypeScript poteto bar: PSR handbook + strict (extends-aware), global-fetch/URL/env + JSON/DOM rg boundaries (method .fetch allowed), portable bare @ts-expect-error, env-schema + typed-parse templates, oxlint adoption wit |
| `python-kit` | [Python Kit](python-kit/) | Dahhrk | Developer Tools | Python poteto bar: PSR PEP 8 / PEP 257 / typing / PyPA encode. One formatter (Ruff format); Ruff lint (E/F/B); mypy or Pyright config; isolate env; test exceptions/I/O/runtime validation. |
| `go-kit` | [Go Kit](go-kit/) | Dahhrk | Developer Tools | Go poteto bar: PSR Effective Go encode. gofmt, go vet, race in CI, propagate errors/cancellation, bound goroutines, close resources, avoid uncontrolled globals. |
| `shell-kit` | [Shell Kit](shell-kit/) | Dahhrk | Developer Tools | Shell poteto bar: PSR Shell encode. ShellCheck, shfmt, quote expansions, set -euo pipefail, safe temps (mktemp+trap), tests for filenames/signals/empty. |
| `rust-kit` | [Rust Kit](rust-kit/) | Dahhrk | Developer Tools | Rust poteto bar: PSR Rust encode. rustfmt, Clippy, cargo test, document unsafe invariants and FFI, avoid unchecked external-boundary assumptions, deliberate app vs library lockfile policy. |
| `c-kit` | [C Kit](c-kit/) | Dahhrk | Developer Tools | C poteto bar: PSR C encode. clang-format, -Wall -Wextra, sanitizers where practical, buffer/unsafe string smells (strcpy/strcat/sprintf/gets), malloc NULL checks. |
| `cpp-kit` | [Cpp Kit](cpp-kit/) | Dahhrk | Developer Tools | C++ poteto bar: PSR C++ encode. clang-format, -Wall -Wextra, clang-tidy where practical, modern C++ smells (raw new/delete, C-style casts, sprintf/vsprintf). |
| `java-kit` | [Java Kit](java-kit/) | Dahhrk | Developer Tools | Java poteto bar: PSR Java encode. google-java-format or spotless (or spring-javaformat), Checkstyle/Error Prone where practical, nullability contracts, SQL/string-concat and System.out smells. |
| `csharp-kit` | [Csharp Kit](csharp-kit/) | Dahhrk | Developer Tools | C# poteto bar: PSR C# encode. dotnet format, Roslyn analyzers, nullable enable, SQL/string-concat and Console.WriteLine-in-libs smells, plus blocking-on-async. |
| `javascript-kit` | [Javascript Kit](javascript-kit/) | Dahhrk | Developer Tools | JavaScript poteto bar (distinct from typescript-kit): PSR JS encode. ESLint flat config, Prettier, no-eval, prototype-pollution smells, sync fs in request path. |
| `ruby-kit` | [Ruby Kit](ruby-kit/) | Dahhrk | Developer Tools | Ruby poteto bar: PSR Ruby encode. RuboCop, rubocop-performance, SQL string interpolate in where/order/select, eval/send smells. |
| `php-kit` | [Php Kit](php-kit/) | Dahhrk | Developer Tools | PHP poteto bar: PSR PHP encode. php-cs-fixer/pint, phpstan/psalm, SQL concat, eval, unserialize smells. Tier 0 single-walk rg + hotpath budget + fmt + phpstan/psalm wiring. Requires ripgrep. |
| `swift-kit` | [Swift Kit](swift-kit/) | Dahhrk | Developer Tools | Swift poteto bar: PSR Swift encode. swift-format, SwiftLint, force unwrap, try!, unsafe pointers. Tier 0 single-walk rg + hotpath budget + fmt + SwiftLint wiring. Requires ripgrep. |
| `kotlin-kit` | [Kotlin Kit](kotlin-kit/) | Dahhrk | Developer Tools | Kotlin poteto bar: PSR Kotlin encode. ktlint, detekt, !! force unwrap, runBlocking on hot paths, SQL concat. Tier 0 single-walk rg + hotpath budget + ktlint + detekt wiring. Requires ripgrep. |
| `zig-kit` | [Zig Kit](zig-kit/) | Dahhrk | Developer Tools | Zig poteto bar: PSR Zig encode. zig fmt, zig build test wiring, @panic/@trap in libs, unchecked alloc (catch unreachable), TODO/FIXME. |
| `elixir-kit` | [Elixir Kit](elixir-kit/) | Dahhrk | Developer Tools | Elixir poteto bar: PSR Elixir encode. mix format, Credo, dialyzer wiring, String.to_atom on input, SQL concat, Process.sleep on hot paths. |
| `sql-kit` | [Sql Kit](sql-kit/) | Dahhrk | Developer Tools | SQL poteto bar: PSR SQL encode. sqlfluff lint, no SELECT *, no SQL injection concat, no unsafe dynamic SQL. Tier 0 single-walk rg + hotpath budget + sqlfluff wiring. Requires ripgrep. |
| `html-kit` | [Html Kit](html-kit/) | Dahhrk | Developer Tools | HTML poteto bar: PSR HTML encode. htmlhint lint, no missing alt, no inline JS/CSS smells, no external script without integrity where relevant. Tier 0 single-walk rg + hotpath budget + htmlhint wiring. Requires ripgrep. |
| `css-kit` | [Css Kit](css-kit/) | Dahhrk | Developer Tools | CSS poteto bar: PSR CSS encode. stylelint lint, no !important abuse, no universal selector hotpath, no expression()/behavior IE smells. Tier 0 single-walk rg + hotpath budget + stylelint wiring. Requires ripgrep. |
| `powershell-kit` | [Powershell Kit](powershell-kit/) | Dahhrk | Developer Tools | PowerShell poteto bar: PSR PowerShell encode. PSScriptAnalyzer lint, no Invoke-Expression, no Write-Host in modules, no unquoted paths. Tier 0 single-walk rg + hotpath budget + PSScriptAnalyzer wiring. Requires ripgrep. |
| `r-kit` | [R Kit](r-kit/) | Dahhrk | Developer Tools | R poteto bar: PSR R encode. lintr lint, no attach(), TRUE/FALSE not T/F, no eval(parse()). Tier 0 single-walk rg + hotpath budget + lintr wiring. Requires ripgrep. |
| `fortran-kit` | [Fortran Kit](fortran-kit/) | Dahhrk | Developer Tools | Fortran poteto bar: PSR Fortran encode. fortitude lint, implicit none, no GOTO, checked I/O (iostat). Tier 0 single-walk rg + hotpath budget + fortitude wiring. Requires ripgrep. fprettify recommended formatter. |
| `assembly-kit` | [Assembly Kit](assembly-kit/) | Dahhrk | Developer Tools | Assembly poteto bar: PSR Assembly encode. No shellcode in product paths, explicit section hygiene, no jmp-to-register without comment gate. |
| `ada-kit` | [Ada Kit](ada-kit/) | Dahhrk | Developer Tools | Ada poteto bar: PSR Ada encode. No Unchecked_Conversion, no pragma Suppress, gnatcheck/gnatpp wiring with Unchecked_Conversions enabled. |
| `objc-kit` | [Objc Kit](objc-kit/) | Dahhrk | Developer Tools | Objective-C poteto bar: PSR ObjC encode. clang-format, ARC (no manual retain/release/autorelease), no NSLog in libs, no performSelector: smells. Tier 0 single-walk rg + hotpath budget + fmt gate. Requires ripgrep. |
| `cobol-kit` | [Cobol Kit](cobol-kit/) | Dahhrk | Developer Tools | COBOL poteto bar: PSR COBOL encode. no GOTO/ALTER, checked ACCEPT (ON EXCEPTION), END-IF hygiene. Tier 0 single-walk rg + hotpath budget + cobc wiring. Requires ripgrep. |
| `delphi-kit` | [Delphi Kit](delphi-kit/) | Dahhrk | Developer Tools | Delphi / Object Pascal poteto bar: PSR Delphi/Pascal encode. no goto, no with-statement, unchecked GetMem banned, WriteLn banned in libs. Tier 0 single-walk rg + hotpath budget + fpc/lazbuild wiring. Requires ripgrep. |
| `vbnet-kit` | [Vbnet Kit](vbnet-kit/) | Dahhrk | Developer Tools | Visual Basic .NET poteto bar: PSR VB.NET encode. On Error Resume Next banned, Option Strict Off banned, Console.WriteLine banned in libs. Tier 0 single-walk rg + hotpath budget + dotnet/vbproj wiring. Requires ripgrep. |
| `slint-kit` | [Slint Kit](slint-kit/) | Dahhrk | Developer Tools | Slint poteto bar: PSR Slint encode. .slint debug() hygiene banned, clone_strong callback capture banned, unsafe blocks in .on_ callback hosts banned. |
| `wasm-kit` | [Wasm Kit](wasm-kit/) | Dahhrk | Developer Tools | WebAssembly poteto bar: PSR Wasm encode. wat hygiene (leftover debug call/import) banned, unbounded memory.grow without comment banned, imported host eval patterns banned. |
| `apps-script-kit` | [Apps Script Kit](apps-script-kit/) | Dahhrk | Developer Tools | Google Apps Script poteto bar: PSR Apps Script encode. eval/new Function banned, Logger.log in libs banned, SpreadsheetApp.getUi (and siblings) in doGet/doPost banned, concurrent sheet writes without LockService banned w |
| `scss-kit` | [Scss Kit](scss-kit/) | Dahhrk | Developer Tools | SCSS/Sass poteto bar: PSR SCSS encode. dart-sass/sass wiring, no !important abuse, no @extend overuse, no /deep/ or >>>, nesting depth ≤4. |
| `astro-kit` | [Astro Kit](astro-kit/) | Dahhrk | Developer Tools | Astro poteto bar: PSR Astro encode. astro check/build wiring, no client:load abuse, no set:html without sanitize, no define:vars XSS smells. Tier 0 single-walk rg + hotpath budget + astro wiring. Requires ripgrep. |
| `mdx-kit` | [Mdx Kit](mdx-kit/) | Dahhrk | Developer Tools | MDX poteto bar: PSR MDX encode. @mdx-js/mdx wiring, no raw HTML injection (dangerouslySetInnerHTML), no untrusted JSX evaluate, no rehype-raw without rehype-sanitize. |
| `pug-kit` | [Pug Kit](pug-kit/) | Dahhrk | Developer Tools | Pug poteto bar: PSR Pug encode. pug wiring, no unescaped buffered XSS (!= / !{}), no include of untrusted interpolated paths, no mixin injection (+#{name}). |
| `tailwind-kit` | [Tailwind Kit](tailwind-kit/) | Dahhrk | Developer Tools | Tailwind CSS poteto bar: PSR Tailwind encode. tailwindcss wiring, no @apply overuse, no arbitrary-value sprawl, no safelist abuse, no content-path miss / purge footguns. |
| `gotemplate-kit` | [Gotemplate Kit](gotemplate-kit/) | Dahhrk | Developer Tools | Go Template poteto bar: PSR Go Template encode. html/template over text/template for HTML (XSS), no Execute without context / discarded err, no missing FuncMap escaping (template.HTML / raw), no nested template include o |
| `mako-kit` | [Mako Kit](mako-kit/) | Dahhrk | Developer Tools | Mako poteto bar: PSR Mako encode. No disable_unicode / input_encoding footguns, no untrusted <%include>, no ${} without filters / \|n raw, no module_directory code-exec cache paths. |
| `dockerfile-kit` | [Dockerfile Kit](dockerfile-kit/) | Dahhrk | Developer Tools | Dockerfile poteto bar: PSR Dockerfile encode. No ADD-vs-COPY secrets, no :latest tags, no apt without cleanup, no USER root late, no secrets in ARG/ENV, no curl\|bash. |
| `cmake-kit` | [Cmake Kit](cmake-kit/) | Dahhrk | Developer Tools | CMake poteto bar: PSR CMake encode. No file(DOWNLOAD) without hash, no unchecked execute_process, no GLOB for sources, no CACHE FORCE abuse, no include of untrusted path. |
| `makefile-kit` | [Makefile Kit](makefile-kit/) | Dahhrk | Developer Tools | Makefile poteto bar: PSR Makefile encode. No recursive make without .PHONY, no tab/space mix, no unchecked $(shell), no include of untrusted path, no .ONESHELL abuse / curl\|bash recipes. |
| `just-kit` | [Just Kit](just-kit/) | Dahhrk | Developer Tools | Just poteto bar: PSR Just encode. No unchecked [script]/shebang recipes, no dotenv secrets in recipes, no export of secrets, no include of untrusted path, no curl\|bash recipes. |
| `nix-kit` | [Nix Kit](nix-kit/) | Dahhrk | Developer Tools | Nix poteto bar: PSR Nix encode. No fetchurl without hash, no builtins.exec / IFD abuse, no impure env lookups, no world-writable store paths in recipes, no curl\|bash in builders. |
| `batchfile-kit` | [Batchfile Kit](batchfile-kit/) | Dahhrk | Developer Tools | Batchfile poteto bar: PSR Batchfile encode. No unquoted %VAR% expansion, no delayedExpansion footguns, no call of untrusted paths, no curl\|powershell download-exec, no secrets in set. |
| `lexyacc-kit` | [Lexyacc Kit](lexyacc-kit/) | Dahhrk | Developer Tools | Lex/Yacc (Flex/Bison) poteto bar: PSR Lex/Yacc encode. No untrusted %include/#include paths, no yyerror silence, no unbounded yytext buffers, no generated C without bounds-checked yytext pointers. |
| `react-kit` | [React Kit](react-kit/) | Dahhrk | Developer Tools | React poteto bar: PSR React encode. react wiring, no dangerouslySetInnerHTML without sanitize, no findDOMNode, no ReactDOM.render (prefer createRoot). |
| `vite-kit` | [Vite Kit](vite-kit/) | Dahhrk | Developer Tools | Vite poteto bar: PSR Vite encode. vite wiring, no server.fs.strict:false, no parent-escape server.fs.allow, no loadEnv empty-prefix all-env dump. Tier 0 single-walk rg + hotpath budget + vite wiring. Requires ripgrep. |
| `gmail` | [Gmail](third_party/gmail/) | Cursor | Productivity | Search, read, draft, and manage email. |
| `google-drive` | [Google Drive](third_party/google-drive/) | Cursor | Productivity | Search, read, create, and share files. |
| `google-calendar` | [Google Calendar](third_party/google-calendar/) | Cursor | Productivity | Search events and schedule meetings. |
| `gong` | [Gong](third_party/gong/) | Cursor | Integrations | Pull account summaries, deal insights, and call briefs. |
| `salesforce` | [Salesforce](third_party/salesforce/) | Cursor | Integrations | Query, create, and update records in your org. |
| `playwright` | [Playwright](third_party/playwright/) | Cursor | Integrations | Navigate, click, screenshot, and test in a real browser. |
| `github` | [GitHub](third_party/github/) | Cursor | Integrations | Manage repos, issues, pull requests, and Actions. |
| `ashby` | [Ashby](third_party/ashby/) | Cursor | Integrations | Search candidates, prep interviews, and manage pipeline tasks. |
| `hubspot` | [HubSpot](third_party/hubspot/) | Cursor | Integrations | Search and update contacts, companies, deals, and tickets. |
| `intercom` | [Intercom](third_party/intercom/) | Cursor | Integrations | Search conversations, contacts, and Help Center articles. |
| `zoom` | [Zoom](third_party/zoom/) | Cursor | Integrations | Search meetings, pull transcripts, and work with Zoom Docs. |
| `x` | [X](third_party/x/) | Cursor | Integrations | Search posts, read timelines, pull trends, and manage bookmarks. |
| `clay` | [Clay](third_party/clay/) | Cursor | Integrations | Enrich people and companies, run AI research agents. |
| `circleback` | [Circleback](third_party/circleback/) | Cursor | Integrations | Search meetings, transcripts, action items, and emails. |
| `docusign` | [Docusign](third_party/docusign/) | Cursor | Integrations | Manage envelopes, templates, workflows, and agreements. |
| `navan` | [Navan](third_party/navan/) | Cursor | Integrations | Query expenses, travel bookings, policies, and cards. |
| `profound` | [Profound](third_party/profound/) | Cursor | Integrations | Track AI visibility, sentiment, and citations. |
| `juicebox` | [Juicebox](third_party/juicebox/) | Cursor | Integrations | Query recruiting analytics, shortlists, and sourcing agents. |
| `outreach` | [Outreach](third_party/outreach/) | Cursor | Integrations | Search sequences, prospects, and Kaia meetings. |
| `amplemarket` | [Amplemarket](third_party/amplemarket/) | Cursor | Integrations | Search people and companies, enrich leads, run sequences. |
| `klaviyo` | [Klaviyo](third_party/klaviyo/) | Cursor | Integrations | Manage profiles, segments, campaigns, and flows. |
| `customer-io` | [Customer.io](third_party/customer-io/) | Cursor | Integrations | Build campaigns, manage segments, and query people. |
| `mailerlite` | [MailerLite](third_party/mailerlite/) | Cursor | Integrations | Manage subscribers, groups, campaigns, and automations. |
| `brevo` | [Brevo](third_party/brevo/) | Cursor | Integrations | Manage contacts, email and SMS campaigns, and CRM deals. |
| `typeform` | [Typeform](third_party/typeform/) | Cursor | Integrations | Build forms, analyze responses, and manage contacts. |
| `jotform` | [Jotform](third_party/jotform/) | Cursor | Integrations | Create and edit forms, then read submissions. |
| `semrush` | [Semrush](third_party/semrush/) | Cursor | Integrations | Research keywords, backlinks, traffic, and competitors. |
| `ahrefs` | [Ahrefs](third_party/ahrefs/) | Cursor | Integrations | Research keywords, backlinks, rankings, and site health. |
| `godaddy` | [GoDaddy](third_party/godaddy/) | Cursor | Integrations | Brainstorm domain names and check availability. |
| `upwork` | [Upwork](third_party/upwork/) | Cursor | Integrations | Search talent, post jobs, and manage contracts. |
| `workable` | [Workable](third_party/workable/) | Cursor | Integrations | Search candidates, move pipelines, and manage HR records. |
| `brex` | [Brex](third_party/brex/) | Cursor | Integrations | Query expenses, receipts, bills, cards, and travel. |
| `mercury` | [Mercury](third_party/mercury/) | Cursor | Integrations | Read balances, transactions, statements, and cards. |
| `todoist` | [Todoist](third_party/todoist/) | Cursor | Integrations | Create, find, and complete tasks and projects. |
| `calendly` | [Calendly](third_party/calendly/) | Cursor | Integrations | Check availability and book, cancel, or reschedule. |
| `smartsheet` | [Smartsheet](third_party/smartsheet/) | Cursor | Integrations | Query and update sheets, rows, and workspaces. |
| `wrike` | [Wrike](third_party/wrike/) | Cursor | Integrations | Search projects, create tasks, and post comments. |
| `coda` | [Coda](third_party/coda/) | Cursor | Integrations | Search docs, read pages, and update tables. |
| `guru` | [Guru](third_party/guru/) | Cursor | Integrations | Search company knowledge and draft verified answers. |
| `fireflies` | [Fireflies](third_party/fireflies/) | Cursor | Integrations | Search meeting transcripts, summaries, and action items. |
| `otter` | [Otter.ai](third_party/otter/) | Cursor | Integrations | Search meeting history and pull full transcripts. |
| `fathom` | [Fathom](third_party/fathom/) | Cursor | Integrations | Search meetings and pull transcripts and summaries. |
| `craft` | [Craft](third_party/craft/) | Cursor | Integrations | Search, create, and update documents and daily notes. |
| `mem` | [Mem](third_party/mem/) | Cursor | Integrations | Capture, search, and organize notes and collections. |
| `readwise` | [Readwise](third_party/readwise/) | Cursor | Integrations | Search highlights and Reader documents, save articles. |
| `similarweb` | [Similarweb](third_party/similarweb/) | Cursor | Integrations | Analyze website traffic, audiences, and competitors. |
| `xero` | [Xero](third_party/xero/) | Cursor | Integrations | Read and write invoices, contacts, reports, and payroll. |
| `x-ads` | [X Ads](third_party/x-ads/) | Cursor | Integrations | Manage ad campaigns, create ads, track conversions, and pull performance stats. |
Author values match each plugin’s `plugin.json` `author.name` (Cursor lists `plugins@cursor.com` in the manifest).

## Repository structure

This is a multi-plugin marketplace repository. The root `.cursor-plugin/marketplace.json` lists all plugins, and each plugin has its own manifest:

```
plugins/
├── .cursor-plugin/
│   └── marketplace.json       # Marketplace manifest (lists all plugins)
├── plugin-name/
│   ├── .cursor-plugin/
│   │   └── plugin.json        # Per-plugin manifest
│   ├── skills/                # Agent skills (SKILL.md with frontmatter)
│   ├── rules/                 # Cursor rules (.mdc files)
│   ├── mcp.json               # MCP server definitions
│   ├── README.md
│   ├── CHANGELOG.md
│   └── LICENSE
└── ...
```

## License

MIT
