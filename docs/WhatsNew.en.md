# What's new

## 0.37.0 — 06.11.2026

- **Installer.** You can now install the app from an MSI file: for yourself without administrator rights, or for all users of the computer, for example on a terminal server. A shortcut appears in the Start menu. The ZIP without installation is still available.
- **Updates from the app.** When a new version comes out, an "Update to …" button appears in the title bar. The app downloads the update, checks the file, installs it and restarts — your dialogs and settings are kept.
- **Update tab.** The settings show the version and how the app is installed; you can check for an update manually and read what is new in the next version.
- **Copyable settings texts.** Messages and statuses in the settings can be selected with the mouse and copied.

## 0.36.0 — 05.11.2026

- **Edit extensions from the chat.** The AI opens an extension module, edits it, checks it with the platform and saves it. A save is confirmed only by 1C's answer; a module with errors is not saved, and you see the error text.
- **Shorter way to an object.** An object visible in the tree is used right away, without a search. "Save" and borrowing no longer make extra checks or wait for nothing.
- **The Designer stays out of the way.** A minimized Designer is minimized again after an operation. A closed main configuration is opened by the operation itself, and a failed read no longer leaves the Designer "busy".
- **Writing code on 1C 8.3.27.** Editing a module on this platform version no longer breaks the work. If the pasted text does not match the expected one, the edit is rolled back automatically and your clipboard is restored.
- **All attributes.** The attribute list is read in full, not only its visible rows. An attribute of an open but covered object can be read too.
- **More reliable with extensions.** Borrowing into an extension that already has many objects is confirmed correctly. An extension tree left over from a previous Designer session no longer breaks reading.
- **Clear chat cards.** A tool card shows a short note about what happened, without instructions for the AI. Right-click to copy its text.

## 0.35.0 — 04.11.2026

- **Proxy.** On the Key tab of the settings you can use the Windows system proxy, connect directly, or set your own proxy with a login and password. It applies immediately, without a restart; "Check" names a clear reason when there is no connection.
- **Tabbed settings.** Key, Billing, AI settings, Markers, General, About and Feedback are listed on the left, as in the Assistant.
- **Billing.** Balance, subscription and its end date, daily and weekly remainders, the key's share and the corporate key mark, with top-up and pricing links — all in one place.
- **No sign-in window.** The app opens the main window right away; without a key the settings open on top of it, so you can set up a proxy before entering the key.
- **Themed dialog title bars.** In the dark theme dialogs no longer open with a white title bar on Windows 10, Windows Server or over Remote Desktop.
- **Clearer refusals.** A deactivated account or organization, a model not on your plan, and a request rejected by the content policy each get their own message. Models outside your plan are shown locked in the list and are never picked automatically.

## 0.34.1 — 04.11.2026

- **Maintenance release.** A new delivery of the accepted 0.34.0 improvements, without changing configurator behavior.

## 0.34.0 — 04.11.2026

- **Fewer unnecessary navigation steps.** Reading reuses the correct open module instead of always reopening the extension and finding the object from the root.
- **Read without switching to the editor.** An available open module can be read without forcing it active.
- **More precise source selection.** Improved reuse of known base-configuration and extension windows, including objects with matching names.
- **Borrow from the open configuration.** No preliminary switch to the extension is required; source tabs in a shared pane are supported.
- **No unnecessary short search limit.** Search reset is confirmed from the actual tree within the overall operation budget. An unconfirmed search is not reported as a missing object.

## 0.33.0 — 29.10.2026

- **Cache in the usage history.** The hourly history now shows cache-read and cache-write columns per model — see how caching shapes the cost. Values appear after the server update; until then the cells show a dash.
- **Cleaner check cards.** A module check without a bound object no longer shows the technical “Module” subtitle — just the title and the check result.
- **Readable dark theme.** Accent action buttons (Save, send) now use white letters on the rose fill.

## 0.32.0 — 29.10.2026

- **Working with an extension.** This workflow is currently manual in the dedicated “1C extensions” window; the AI does not yet manage extensions directly. The buttons let you create an extension, adopt an object, read its module, prepare a change, check it with the platform and explicitly save. The window shows which extension owns the code.
- **A local draft.** Edit a module as text or in exported files. Your draft is saved separately; a conflict with live 1C code stops application and preserves your edits.
- **Background actions in Designer 8.5.** Reading, sending code, platform checks and extension commands run without switching to the 1C window. An uncertain outcome is reported separately and is never retried automatically.
- **Additional BSL checks.** An optional component checks code and coding standards in the sandbox and local module. Settings let you install it, inspect its state and remove it. Platform checks remain available separately.
- **The actual open window.** The active module follows the current 1C state; an unknown name is explicitly marked in the window list.

Extension commands for the AI will become available after the server update.

## 0.31.0 — 25.10.2026

- **Hourly usage history.** Settings show how many calls, tokens and coins each hour took — separately for every AI model. Times follow your computer's clock.
- **A clear key limit refusal.** When a key has a spending ceiling and it is used up, the app says which limit ran out — daily, weekly or total — how much is left and when it renews. The coins in your account are untouched.
- **Key limit instead of balance.** When the key may spend less than the account holds, the header shows the key's available remainder; the tooltip names both amounts.

## 0.30.1 — 25.10.2026

- **A larger header.** The logo, name, version and connection status are bigger and fit on one line; header buttons are larger and easier to hit.
- **No stray icon in window titles.** Settings, Help and other windows no longer show a tiny icon in the title bar; the taskbar keeps it.
- **The product logo in an empty dialog.** A new dialog opens with a large logo.
- **The context ring is always visible.** The ring next to the composer stands out in every theme. In an empty dialog its tooltip shows the selected AI model's context size; when it is unknown, it says so instead of showing zero.
- **A tidier configurator list.** Infobases are split into "Open" and "Recent". You can remove a recent infobase from the list or hide an open one; both ask for confirmation. Hidden infobases come back from a collapsed section. 1C itself, the infobase and its dialogs are not affected.
- **An arrow on the Send button.** Send is an up arrow; in the 1C theme the button is raspberry, as in the light theme.
- **A clean dialog history.** Internal server records no longer show up in the history as unreadable text.

## 0.29.0 — 23.10.2026

- **Open EPF names.** Refresh and chat tools identify open EPF modules and switch to the selected window.
- **More reliable module edits.** After pasting, the client confirms the text landed in the right module. When 1C gives no sign whether an edit went through, the client says so and does not suggest pasting it again blindly.
- **Check the open module.** The native 1C syntax check also works with external EPF modules, without restrictions based on the file name or module kind.
- **Current procedure in chat.** The client reads the live module's caret after you return to the composer. When 1C does not expose an exact position, it is left unspecified.

## 0.28.0 — 23.10.2026

- **Updated icon.** A lens, laptop and “1”, with a dark outline; the dark theme adds a raspberry separator above the keyboard.
- **Change your key in Settings.** Validate, apply or cancel in the same window. A failed check keeps your previous key; its status and balance are labelled separately from the new key's check result.
- **More room in Settings.** More spacing between fields, a readable comment preview, and the coin symbol after the amount.
- **Plan, Review and Trust.** A page and pencil, magnifier and outlined handshake, in blue, purple and green. Review still prepares edits in the sandbox.
- **Readable text.** Popup headings, links, errors and status text have better contrast. A narrow composer shortens the model name to keep Send visible.
- **Updated Help.** A larger logo and full product name, with clearer Russian terminology in the user guide.

## 0.27.0 — 22.10.2026

- **An individual attribute's type from the 1C property palette.** String length, numeric precision, date, boolean and observed reference types. The name, synonym and comment remain available even when the type cannot be read.
- **No guessing from names.** Composite, unknown and unreadable types are identified explicitly. Attribute lists still do not contain types.

## 0.26.0 — 21.10.2026

- **New colors and distinct surfaces.** Light and dark themes use a raspberry accent; the board, feed and composer are separated. The input has a focus border, and Auto stays green.
- **Settings in one window.** A masked key with temporary reveal, status and balance, connection check, useful links and the existing marker options.
- **Feedback from the app.** Send a review, report or feature request from Settings; a failed send keeps your draft.
- **Quote a selected phrase.** Select text in a reply and click Quote. The caret moves into the composer, and the reply footer stays visible as the input grows.
- **Themed confirmations.** Delete a task, change a key or add code to the sandbox. The info button matches its neighboring actions.

## 0.25.0 — 21.10.2026

- **Properties of one attribute.** The app reads the name, synonym and comment from a catalog or document attribute's property palette. Attribute types are the next step.
- **Fewer configurator transitions.** Opening an object module reuses the editor already open for the requested object.
- **Read messages are cleared.** After a complete panel read or a confirmed successful check, old messages no longer accumulate. The panel stays intact when an error is found.
- **Window captions follow the theme.** Help, Settings and other dialogs remain readable in dark, light and 1C themes, including when inactive.

## 0.24.0 — 17.10.2026

- **What's new and Planned right in Help.** After an update the app shows once what has changed.
- **Full dialog names.** Names are no longer cut at 40 characters. A few seconds after the reply the server gives the dialog a short meaningful name; hover over a history row to see the full name.
- **Coins stand out.** An amber coin icon next to the balance, and coins are the last column in dialog properties.

## 0.23.0 — 17.10.2026

- **The model checks a module itself.** It runs the configurator's standard module check, reads the Messages panel and fixes the error it found. It reports success only when the platform explicitly confirms there are no errors.
- **Object attributes by address.** Ask about the attributes of a catalog or document and the app reads only them, without walking forms and templates.
- **An open module is not searched for again.** If the needed object module is already active, the model works in it right away.
- **The app window no longer covers the configurator.** While the model works in 1C, "always on top" is lifted and comes back when you return to the app.
- **Model names are readable in every theme.**

## 0.22.0 — 15.10.2026

- **Open a catalog or document by name.** "Open the object module of catalog Контрагенты" — the model finds the object in the configurator and opens the module itself.
- **Object description.** Attributes, tabular sections, forms and templates of an object, read from the configurator's editor window. What is not visible, the model does not make up.
- **1C actions do not collide.** Only one chat drives the configurator at a time, and an action in the history without a confirmed result is not repeated.

## 0.21.0 — 12.10.2026

- **New header.** Version next to the name, connection status, balance with a top-up button and a connection check button.
- **Dialog properties.** Name, spending per model, deletion and export of the dialog to Markdown.
- **Offline help** — the "?" button in the header.
- **One frame per model turn.** Tool steps and the final answer are grouped; model, time, copy and quote sit in the line above the answer.

## 0.20.0 — 12.10.2026

- **Compact the context by clicking the ring.** If compaction is not possible, the tooltip says why.
- **The model sees where you are in the sandbox.** The procedure or selected fragment under the caret goes into the request — without the whole module text.
- **Task boards of other dialogs.** The model can look into the boards of neighbouring dialogs of its database.
- **Reasoning levels from the model catalog** and detailed metrics of every turn: coins, tokens, cache, time.

## 0.19.0 — 17.08.2026

- **A module from disk — without the configurator.** The sandbox got "Open file…" and "Save as…": a dump, an EDT file or someone else's code open right in the editor, and the encoding is detected automatically.
- **A long message is not cut silently.** A length counter appears near the limit and prevents sending text that is too long.

## Earlier

- **Configurator operator.** The model reads and edits code in the open configurator window, and changes are marked.
- **Sandbox with a code editor.** 1C highlighting, region folding, moving finished code to the configurator window with one button.
- **Task board.** The model plans work on the board, you edit it by hand, and the plan survives a restart.
- **Edit check.** A model edit is not written if it breaks parsing of the module.
- **One file.** The app ships as a single EXE together with its own editor engine.
