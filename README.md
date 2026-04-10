# All of Create — Custom Modpack

A customized version of the [All of Create](https://www.curseforge.com/minecraft/modpacks/all-of-create) modpack with additional mods for our server.

- **Minecraft:** 1.20.1
- **Mod Loader:** Forge 47.4.2

---

## First Time Setup

Follow the instructions for your launcher below.

---

### 🟦 Prism Launcher

**Step 1 — Create a new instance**
1. Open Prism Launcher and click **Add Instance**
2. Select **Minecraft 1.20.1** with **Forge 47.4.2** as the mod loader
3. Name it something like `All of Create`
4. Click **OK**

**Step 2 — Add the bootstrapper**
1. Download [`packwiz-installer-bootstrap.jar`](https://github.com/packwiz/packwiz-installer-bootstrap/releases/latest)
3. Click **Open Folder** on your instance to open its `.minecraft` folder
4. Place `packwiz-installer-bootstrap.jar` directly in that folder

**Step 3 — Add the pre-launch command**
1. Still in **Edit Instance**, go to **Settings → Custom commands**
2. Check **Use custom commands**
3. Paste this into the **Pre-launch command** field:
```
"$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/noahhaon05/All-of-Create-CUSTOM/main/pack.toml
```

**Step 4 — Launch**

Launch the instance. The bootstrapper will automatically download all mods on first launch. This may take a few minutes.

---

### 🟧 ATLauncher

**Step 1 — Create a new instance**
1. Open ATLauncher and go to the **Vanilla Packs** tab
2. Click **New Instance**
3. Select **Minecraft 1.20.1** and choose **Forge 47.4.2** as the loader
4. Name it `All of Create ` and click **Create Instance**

**Step 2 — Add the bootstrapper**
1. Download [`packwiz-installer-bootstrap.jar`](https://github.com/packwiz/packwiz-installer-bootstrap/releases/latest)
2. Click **Open Folder** on your instance to open its `.minecraft` folder
3. Place `packwiz-installer-bootstrap.jar` directly in that folder

**Step 3 — Add the pre-launch command**
1. Click the **Settings** on your instance
2. Go to **Commands**
3. Change **Enable commands?** to **Yes**
4. Find **Pre-launch command**
5. Paste this:
```
javaw -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/noahhaon05/All-of-Create-CUSTOM/main/pack.toml
```

**Step 4 — Launch**

Launch the instance. All mods will download automatically on first launch.

---

### 🟪 CurseForge App

CurseForge does not support automatic updates via the bootstrapper. Follow these steps to install manually.

**Step 1 — Download the modpack zip**
1. Go to the [Releases page](https://github.com/noahhaon05/All-of-Create-CUSTOM/releases/latest)
2. Download the latest `modpack.zip`

**Step 2 — Import into CurseForge**
1. Open the CurseForge App and go to **Minecraft**
2. Click **Create Custom Profile** → **Import**
3. Select the downloaded `modpack.zip`
4. CurseForge will automatically download all mods — this may take a few minutes

**Step 3 — Play**

Once installed, launch the profile from CurseForge as normal.

> 💡 **Tip:** Consider switching to [Prism Launcher](https://prismlauncher.org/) or [ATLauncher](https://atlauncher.com) (free) for fully automatic updates — no manual steps needed when the modpack changes.

---

## Updating the Modpack

### 🟦 Prism Launcher & 🟧 ATLauncher

**Nothing to do.** The bootstrapper checks for updates every time you launch. If there are changes, it downloads them automatically before the game starts.

---

### 🟪 CurseForge App

You need to re-import the modpack zip when there's an update.

**Step 1 — Download the new zip**
1. Go to the [Releases page](https://github.com/noahhaon05/All-of-Create-CUSTOM/releases/latest)
2. Download the latest `modpack.zip`

**Step 2 — Import the update**
1. Open the CurseForge App and go to **Minecraft**
2. Click **Create Custom Profile** → **Import**
3. Select the newly downloaded `modpack.zip`

> ⚠️ **Note:** Importing creates a new profile rather than updating the existing one. You can delete the old profile after confirming the new one works. To have your previous configured configs, saves, JEI and waypoints you might have to copy some folders/files.

---

## Troubleshooting

**Mods not downloading on launch (Prism/ATLauncher)**
- Make sure `packwiz-installer-bootstrap.jar` is in the correct folder (the `.minecraft` folder of your instance)
- Double-check the pre-launch command is set correctly and matches the URL above exactly

**Game crashes on startup**
- Make sure you're using **Forge 47.4.2** specifically — other Forge versions may not be compatible
- Check that you haven't added extra mods that conflict with the modpack

**CurseForge zip won't import**
- Make sure you downloaded the zip from the [Releases page](https://github.com/noahhaon05/All-of-Create-CUSTOM/releases/latest) and not the source code zip
