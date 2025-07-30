### Zen Mods

- Animation Plus
- Better Unloaded Tabs
- Cleaner Extensions
- Custom uiFont
- Disable Status Bar
- Hide Extension Name
- Hide Window Buttons
- Load Bar
- NavBar Margins
- No Search Shortcut Icons
- No Sidebar Scrollbar
- Transparent Zen

### Flags

These are the flags manually set in the `about:config` page of the browser.

- `devtools.chrome.enabled`: `true`
- `devtools.debugger.remote-enabled`: `true` - enables inspecting the Zen window itself via `ctrl+alt+shift+i`
- `toolkit.legacyUserProfileCustomizations.stylesheets`: `true`
- `zen.view.experimental-no-window-controls`: `true`

Add custom flags.

- `zen.browser.is-cool`: `true`

### Extensions

- [Stylus](https://addons.mozilla.org/en-US/firefox/addon/styl-us)
- [uBlock origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin)
- [Vimium C](https://addons.mozilla.org/en-US/firefox/addon/vimium-c)

#### How to apply theme using Stylus?

##### Fonts and Colors

Requirements:

- `go`
- `make`

Download and install browser extension **Stylus**.

- <a href="https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne" target="_blank">Stylus for Chrome</a>
- <a href="https://addons.mozilla.org/en-US/firefox/addon/styl-us" target="_blank">Stylus for Firefox</a>

Clone the repository and build the `.scss` file

- `git clone https://github.com/nobilissimum/apps`
- `cd zen-browser/extensions/stylus`
- `make build`
- `./run`

Click the **Stylus** extension in the browser's extensions panel then select <kbd>Manage</kbd>. There's a <kbd>Write new style</kbd> option in the side menu under the **Backup** section. This will create a new blank style. Select the <kbd>Import</kbd> button in the side menu then paste the contents of `dist.scss` then click <kbd>Overwrite style</kbd>.

#### Supported websites with Hush colors

- https://www.github.com
- https://www.linkedin.com
- https://www.twitch.tv
- https://twitter.com and https://x.com

##### Sidebar Tab Groups

Go to `about:profiles` and navigate to the **root directory** of the preferred profile. You may click on the _Open Folder_ button. Create a directory named `chrome` if it doesn't exist and copy-paste `userChrome.scss` as `userChrome.css` file.

### References

- [Live Editing Zen Theme](https://docs.zen-browser.app/guides/live-editing)
