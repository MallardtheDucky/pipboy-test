PIP-BOY 3000A  //  FALLOUT: NEW VEGAS CHARACTER SHEET
Open index.html in a browser (double-click works; no server required).
Keys: Q/E main tab, Left/Right sub tab, Up/Down select, +/- adjust, Enter use/equip, 1/2 weapon slot, M mute.
Progress autosaves to localStorage. DATA > BIO > RESET ALL DATA wipes it.

UPDATE NOTES
- Status screen now uses the Vault Boy Paper Doll textures (assets/images/doll/).
  Each limb is its own outline; a crippled (0%) limb swaps to its dashed "_broken"
  version, injured limbs (<50%) dim, and the face changes with HP / radiation.
  Set VAULT_BOY_STYLE = 'image' at the top of the doll block in app.js to go back
  to the single assets/images/vault_boy.png.
- Crippled limbs show a CRIPPLED label instead of a bar, and the radiation meter
  wobbles slightly (both mirror the stock stats_menu.xml behaviour).
- There are no on-screen controls for changing HP, limbs or rads, and the
  "+/- ADJUST" hint is hidden on the Status screen.

ICON UPDATE
- New icon library from interface.rar, converted to PNG: assets/images/icons/ (items, apparel, weapons,
  perks, skills, derived stats, karma, factions). icons.js lists the files that exist.
- Items/Perks/Skills detail panes now show their icon. Items are matched by name, so newly
  created items pick up an icon automatically when their name resembles a known one.
- New STATS > General sub-tab: Karma, 13 faction Reputations (+/- to adjust) and Derived Statistics.
  Karma and reputations autosave with the rest of the sheet.
- interface.rar was partly damaged: 4 files could not be recovered (perk_entomologist,
  perk_scrounger, perk_survival guru, skills_survival) and are not included.

CASING + PORTRAIT UPDATE
- The screen now sits in a gold Pip-Boy casing (wide screens). The STATS / ITEMS / DATA buttons work and the
  rad gauge needle follows your RADS. On narrow screens the casing hides and the screen fills the window.
- Fixed the boxy glow behind the Vault Boy (a selection rectangle); limbs now just glow.
- Character portrait: DATA > Bio > Portrait to upload an image (Terminal Tint toggles the amber look).
  It also shows on STATS > Status > General. Stored in this browser only; RESET ALL DATA removes it.
