CoreSwitch
README EN / Distribution Guide
============================================================

v3.0.15

■ Introduction

CoreSwitch is a Windows application developed in Japan to make everyday tasks
quicker. Use it to reuse something you copied earlier, separate windows by task,
transfer custom words between a PC and a phone, or switch between Japanese
and alphanumeric input. The four tools can be launched individually from the
main window, called the Commander.
Find the installed version at the bottom of that window or under Help > About.
Japanese interface labels are included below to help you follow the English guide.

■ System Requirements

This package is intended for 64-bit Windows 11. The main application,
Dictionary Core, and Virtual Desktop Tool run with standard privileges.
ClipSel and Alt-Space require administrator approval at launch.

■ Included Modules

- ClipSel v4.1.8 retrieves previously copied text and images and stores reusable snippets.
- Virtual Desktop Tool v2.0.0.4 changes workspaces with keyboard shortcuts.
- Dictionary Core v2.3.0 edits custom word lists and prepares them for another input app.
- Alt-Space v3.2.11 switches input modes with Alt, a long press of Space, or conversion keys.

■ Getting Started

1. Extract the entire ZIP. Keep CoreSwitch.exe beside the Modules folder
   and preserve the executable names and folder layout.
2. Open CoreSwitch.exe. Select Launch (起動) beside a module, or Start Resident
   Modules (常駐モジュールを起動) to start the three resident tools together.
   To open Dictionary Core, use its own Launch button.
3. When Windows requests administrator approval for ClipSel or Alt-Space,
   check the application name before approving.

Use Commander Settings (司令塔設定) to choose whether CoreSwitch starts with
Windows and which resident modules start automatically. The window's close
button hides it. Use Exit Commander (司令塔を終了) to exit CoreSwitch.

■ Try ClipSel in a Minute

1. Click Launch (起動) beside ClipSel. Open Notepad, type “apple” and “orange”,
   and copy each word separately with Ctrl+C.
2. Click in Notepad where you want to paste, then press Ctrl+Shift+U.
   The History (履歴) tab opens with the most recent copy, “orange”, at the top.
3. Double-click the “apple” row. The word appears in Notepad. Press Ctrl+Shift+U
   to reopen the list, or Esc to hide it.

■ Find, Order and Paste Clipboard Items

ClipSel captures supported items you copy while it is running. As well as
retrieving old text, you can assemble notes or insert a reusable greeting.
Saving, searching and scrolling were tested with one million sample text entries.
Speed and disk usage depend on your PC and the contents of your history.

- Type in the search box to search the entire history. Up to 100 matches appear,
  with exact matches first, followed by prefix matches and then other matches.
  Clear the box to restore the full list. Use the wheel or scrollbar to browse
  from the newest item to the oldest without switching pages.
- To paste nonadjacent rows in your own order, click the first row, then hold
  Ctrl and click the others. Press Enter to paste the text on separate lines.
  Clicking row 8, then Ctrl-clicking rows 3 and 6, gives 8, 3, 6. Deselecting
  an item and selecting it again moves it to the end of the paste order.
- For a continuous range, click the first row, then Shift-click the last.
  Enter pastes the rows from top to bottom. To choose items using the keyboard,
  focus the list, move with the arrow keys, mark items with Space, and press Enter.
- Press Ctrl+Shift+Y to paste items one at a time while keeping ClipSel available.
  While the ClipSel window is open, press Ctrl+Y to enable continuous paste or
  Ctrl+U to return to single paste.
  Save reusable text with the New button on the Snippets (定型文) tab, then
  double-click the snippet to insert it.
- Paste images one at a time. Files copied from Explorer must still exist at
  their original locations when you paste them.
- To delete items, right-click inside the selection, choose Delete, and check
  the count before confirming. The items disappear from browsing, search and
  paste after a restart as well. Their underlying text and attachments remain
  on disk. Clear All History removes all stored history entries and attachments.

■ Switch Workspaces with Virtual Desktop Tool

Windows virtual desktops let you group windows by task on one PC. For example,
you can keep reference material on one desktop and a writing app on another.
Press Alt+I to create a desktop, Alt+K to move left, Alt+O to move right,
and Alt+L to close the current desktop.

■ Switch Between Japanese and Alphanumeric Input with Alt-Space

Start Alt-Space and press Ctrl+Alt+I to open its settings. Under Basic Style
(基本スタイル), choose an Alt tap, a long press of Space, or both. For an Alt tap,
choose the left key, the right key, or both. On a Japanese keyboard, you can
select IME Switching (IME切り替え) for the Henkan and Muhenkan keys. Click
Apply (設定を適用) when ready. An optional on-screen display shows the input
mode in the center of the screen. The Google Japanese Input indicators “あ”
and “A” near the text cursor were also confirmed on the test PC.

If Google Japanese Input shows "_A" (half-width alphanumeric while the IME is
on), press a key assigned to IME switching in Alt-Space once. On the test PC,
Alt, Henkan and Muhenkan each restored Hiragana. If switching fails, try the
keyboard's Kana key (カナ／かな) to return to Japanese input.

■ Share Your Custom Words with Dictionary Core

A user dictionary stores words such as names, addresses and technical terms
under short readings. Dictionary Core opens a file exported by your original
input app and saves a file that the destination app can import. For example,
you can transfer custom words from Google Japanese Input on a PC to flick on
a phone. Transfer the exported file to the destination device and import it
in the destination input app.

■ ATOK Word List Conversion (Beta)

Dictionary Core converts files between ATOK, Google/Mozc, MS IME, Simeji,
and flick. Export an ATOK text word list from the ATOK Dictionary Utility,
then open it with the ATOK beta button (ATOK（ベータ）). To transfer words
back to ATOK, choose Save to ATOK (ATOKへ保存（ベータ）) and import the
saved text file in the ATOK Dictionary Utility. Output uses UTF-16LE with a BOM.

Readings and words are converted. Parts of speech and comments are carried
over where the destination format supports them. Before saving, the app
warns when a part of speech will become a noun or when data such as
replacement candidates or language tags will be omitted. Keep the original
dictionary. File conversion across all five formats was tested with sample
data. Import into ATOK and compatibility with every IME or device version
remain unverified. Try importing a small sample into a separate dictionary first.

■ 60-Minute Trial and License Activation

An unregistered installation has a 60-minute cumulative trial. Registering
the issued key removes the time limit. The key is tied to the Machine ID
used in your request. To unregister it, choose Remove License and Return to
Trial (ライセンスを削除して試用版に戻す). Any trial time already used is carried over.
You can register your key again on a PC with the same Machine ID.
Starting with v3.0.9, CoreSwitch uses signed keys beginning with CS1-.
For a replacement of an older key, contact support with your Machine ID and order number.

1. Open License (ライセンス) > License Registration and Management (ライセンス登録・管理).
2. After purchasing on BOOTH, follow the registration window's instructions
   to send your Machine ID and BOOTH order number. You can copy the request
   template or open a draft in your email application.
3. Enter the issued key and select Verify and Register (認証して登録).

BOOTH  https://masatech.booth.pm/
License requests and support  masatech.dev.apps@gmail.com

■ Help and Updates

Open Help (ヘルプ) > User Guide (English) to read this guide in the app.
About shows the installed version and support contact.

■ Update Notifications and Updating in Place

1. Download the new distribution ZIP and extract it into a separate location.
2. In the running copy of CoreSwitch, click Exit Commander (司令塔を終了).
   Wait for its modules to exit.
3. Copy the contents of the extracted CoreSwitch folder into the folder that
   contains your existing CoreSwitch.exe. Choose “Replace the files” when Windows
   asks, then open CoreSwitch.exe from its usual location.

Keep the existing folder. The distribution ZIP contains no personal history,
snippets or settings, so you can leave them in place during the update.
CoreSwitch checks for a public GitHub release at startup. When a newer version
is available, it offers to open the download page. To check manually, choose
Help > Check Updates on GitHub (GitHubで更新を確認).

■ Troubleshooting

Launch modules from the CoreSwitch main window. If a launch authorization error
persists, confirm that the main executable is named CoreSwitch.exe and is beside
the Modules folder. When contacting support, include the version, module name,
and error message. Launch logs are under %AppData%\MasaTech\CoreSwitch\Diagnostics.
Review logs before sharing. License keys and clipboard history are unnecessary.

■ Data Location and Removal

ClipSel stores its history and snippets under Modules\Data or
%LocalAppData%\MasaTech\CoreSwitch\ClipSel\Data. Commander settings are stored
under %AppData%\MasaTech\CoreSwitch. To remove the application, disable Windows
startup registration in Commander Settings and choose Exit Commander. If you
want to use your history and snippets later, copy the Data folder to a separate
location before deleting the extracted application folder. You can manage the
settings and data stored in AppData separately.

■ Distribution Files and Third-party Software

- CoreSwitch.exe and Modules contain the main application and four modules.
- README_JP.txt and README_EN.txt provide Japanese and English instructions.
- THIRD_PARTY_NOTICES.txt lists third-party software and license references.
- source contains AutoHotkey and Ahk2Exe/BinMod source materials and notes
  on the protection process.

Open License (ライセンス) > Third-party Licenses (第三者ライセンス) to read the
notice and full license texts in the app. Third-party software remains subject to its own license terms.
Product terms do not restrict the rights those licenses grant.

Developed by MasaTech / Itachi, Spica and Mahiru
Support  masatech.dev.apps@gmail.com
