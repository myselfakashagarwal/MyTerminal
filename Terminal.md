# Terminal 

The terminal I use it the [Tabby](https://tabby.sh/) for your setup Just download the Tabby and goto settings > config file and paste the configurations also please consider that ⌘ key of mac is an alias for Super key in non mac keyboards 

```
version: 7
profiles: []
groups: []
configSync:
  parts: {}
hotkeys:
  toggle-window: []
  copy-current-path: []
  ctrl-c:
    - Ctrl-C
  copy:
    - ⌘-C
  paste:
    - ⌘-V
  clear:
    - ⌘-K
  select-all:
    - ⌘-A
  zoom-in:
    - ⌘-=
    - ⌘-Shift-=
  zoom-out:
    - ⌘--
    - ⌘-Shift--
  reset-zoom:
    - ⌘-0
  home:
    - ⌘-Left
    - Home
  end:
    - ⌘-Right
    - End
  previous-word:
    - ⌥-Left
  next-word:
    - ⌥-Right
  delete-previous-word:
    - ⌥-Backspace
  delete-line:
    - ⌘-Backspace
  delete-next-word:
    - ⌥-Delete
  search:
    - ⌘-F
  pane-focus-all:
    - ⌘-Shift-I
  focus-all-tabs:
    - ⌘-⌥-Shift-I
  scroll-to-top:
    - Shift-PageUp
  scroll-up:
    - ⌥-PageUp
  scroll-down:
    - ⌥-PageDown
  scroll-to-bottom:
    - Shift-PageDown
  restart-telnet-session: []
  restart-ssh-session: []
  launch-winscp: []
  settings-tab: {}
  settings:
    - ⌘-,
  serial:
    - Alt-K
  restart-serial-session: []
  new-tab:
    - ⌘-T
  new-window:
    - ⌘-N
  profile: {}
  profile-selectors: {}
  toggle-fullscreen:
    - Ctrl+⌘+F
  close-tab:
    - ⌘-W
  reopen-tab:
    - ⌘-Shift-T
  toggle-last-tab: []
  rename-tab:
    - ⌘-R
  next-tab:
    - Ctrl-Tab
  previous-tab:
    - Ctrl-Shift-Tab
  move-tab-left:
    - ⌘-Shift-Left
  move-tab-right:
    - ⌘-Shift-Right
  rearrange-panes:
    - Ctrl-Shift
  tab-1:
    - ⌘-1
  tab-2:
    - ⌘-2
  tab-3:
    - ⌘-3
  tab-4:
    - ⌘-4
  tab-5:
    - ⌘-5
  tab-6:
    - ⌘-6
  tab-7:
    - ⌘-7
  tab-8:
    - ⌘-8
  tab-9:
    - ⌘-9
  tab-10: []
  duplicate-tab: []
  restart-tab: []
  reconnect-tab: []
  disconnect-tab: []
  explode-tab:
    - ⌘-Shift-.
  combine-tabs:
    - ⌘-Shift-,
  tab-11: []
  tab-12: []
  tab-13: []
  tab-14: []
  tab-15: []
  tab-16: []
  tab-17: []
  tab-18: []
  tab-19: []
  tab-20: []
  split-right:
    - ⌘-Shift-D
  split-bottom:
    - ⌘-D
  split-left: []
  split-top: []
  pane-nav-right:
    - ⌘-⌥-Right
  pane-nav-down:
    - ⌘-⌥-Down
  pane-nav-up:
    - ⌘-⌥-Up
  pane-nav-left:
    - ⌘-⌥-Left
  pane-nav-previous:
    - ⌘-⌥-[
  pane-nav-next:
    - ⌘-⌥-]
  pane-nav-1: []
  pane-nav-2: []
  pane-nav-3: []
  pane-nav-4: []
  pane-nav-5: []
  pane-nav-6: []
  pane-nav-7: []
  pane-nav-8: []
  pane-nav-9: []
  pane-maximize:
    - ⌘-⌥-Enter
  close-pane:
    - ⌘-Shift-W
  pane-increase-vertical: []
  pane-decrease-vertical: []
  pane-increase-horizontal: []
  pane-decrease-horizontal: []
  profile-selector:
    - ⌘-E
  switch-profile:
    - ⌘-Shift-E
  command-selector:
    - ⌘-Shift-P
  search-in-browser: []
terminal:
  searchOptions: {}
  colorScheme:
    name: base2tone-meadow-dark
    foreground: '#ffffff'
    background: rgb(0, 0, 0)
    cursor: '#00838f'
    colors:
      - '#dce775'
      - '#fff176'
      - '#4db6ac'
      - '#a6f655'
      - '#0288d1'
      - '#ffffff'
      - '#aed581'
      - '#0288d1'
      - '#00838f'
      - '#8cdd3c'
      - '#223644'
      - '#335166'
      - '#466b86'
      - '#ad1457'
      - '#c2185b'
      - '#4db6ac'
  customColorSchemes:
    - name: base2tone-meadow-dark
      foreground: '#ffffff'
      background: rgb(0, 0, 0)
      cursor: '#4d8217'
      colors:
        - '#dce775'
        - '#fff176'
        - '#80bf40'
        - '#a6f655'
        - '#0288d1'
        - '#0097a7'
        - '#9e9d24'
        - '#0288d1'
        - '#00838f'
        - '#8cdd3c'
        - '#223644'
        - '#335166'
        - '#466b86'
        - '#a5d6a7'
        - '#73b234'
        - '#4db6ac'
    - name: dull color
      foreground: '#7ba8b7'
      background: rgb(0, 0, 0)
      cursor: '#81c784'
      colors:
        - '#7b1fa2'
        - '#3e91ac'
        - '#00695c'
        - '#fdd835'
        - '#499fbc'
        - '#37474f'
        - '#62b1cb'
        - '#7ba8b7'
        - '#3d6876'
        - '#afb42b'
        - '#223c44'
        - '#335966'
        - '#467686'
        - '#a5d8e9'
        - '#c4b031'
        - '#e1f7ff'
  linePadding: 4
  profile: local:binbash
  hideTabIndex: true
  autoOpen: false
  bell: audible
  fontSize: 25
  paneResizeStep: 0.5
  lightColorScheme:
    name: Tabby Default Light
    foreground: '#4d4d4c'
    background: '#ffffff'
    cursor: '#4d4d4c'
    colors:
      - '#000000'
      - '#c82829'
      - '#718c00'
      - '#eab700'
      - '#4271ae'
      - '#8959a8'
      - '#3e999f'
      - '#ffffff'
      - '#000000'
      - '#c82829'
      - '#718c00'
      - '#eab700'
      - '#4271ae'
      - '#8959a8'
      - '#3e999f'
      - '#ffffff'
  font: JetBrainsMono Nerd Font Mono
ssh: {}
clickableLinks: {}
accessibility:
  animations: false
appearance:
  dockFill: 1
  dockScreen: 1
  dockAlwaysOnTop: false
  spaciness: 1.2
  frame: full
  tabsInFullscreen: true
  colorSchemeMode: auto
hacks: {}
providerBlacklist: []
commandBlacklist: []
language: en-GB
enableAnalytics: false
enableWelcomeTab: false
profileBlacklist:
  - local:default
profileDefaults:
  ssh:
    disableDynamicTitle: true
  local:
    type: local
    options:
      env:
        PS1: '"\u @ \w :"'
recoverTabs: false
searchInBrowserPlugin: {}
pluginBlacklist: []

```