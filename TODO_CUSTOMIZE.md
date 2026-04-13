# Personalization Checklist

A comprehensive list of every file and asset you need to change to make this 3D portfolio your own. 

## 1. Root Configuration & Documentation
- [ ] **`package.json`**: Update `"name"`, `"author"`, `"repository"`, `"bugs"`, and `"homepage"`.
- [ ] **`package-lock.json`**: Update `"name"` to match `package.json`.
- [ ] **`readme.md`**: Update the title, description, and social image links.
- [ ] **`license.md`**: Change `Copyright (c) 2025 Bruno Simon` to your own name.

## 2. HTML & SEO Meta Tags
- [ ] **`sources/index.html`**:
  - [ ] `<title>`: Change "Bruno's" to your title.
  - [ ] `<meta name="description">`: Update description.
  - [ ] `<meta itemprop="name" / "description" / "image">`: Update schema tags.
  - [ ] `<meta name="twitter:...">`: Update Twitter card title, description, image, and domain.
  - [ ] `<meta property="og:...">`: Update Open Graph URL, title, description, and image.
  - [ ] Google Analytics script at the bottom: Update the `G-XXXXXXXX` ID or remove the script entirely.

## 3. Content Data (Text & Links)
- [ ] **`sources/data/consoleLog.js`**: 
  - [ ] Change the big ASCII art comment header.
  - [ ] Update URLs and details for Mail, X, BlueSky, YouTube, Twitch, GitHub, LinkedIn.
- [ ] **`sources/data/social.js`**: Update your social media links that appear as 3D interactive points.
- [ ] **`sources/data/projects.js`**: Swap out Bruno's portfolio work for your own (names, links, descriptions, image paths).
- [ ] **`sources/data/lab.js`**: Replace the experiments/side-projects.
- [ ] **`sources/data/achievements.js`**: Customize or rename the interactive achievements.

## 4. Images & Static Assets
- [ ] **`static/favicons/`**: Replace `android-chrome-*.png`, `apple-touch-icon.png`, `favicon-*.png`, `favicon.ico`, `mstile-*.png`, `safari-pinned-tab.svg` with your own branding. Include updates to `browserconfig.xml` and `site.webmanifest` if necessary.
- [ ] **`static/social/share-image.png`**: Replace with your own preview image for social sharing.
- [ ] **`static/projects/`**: Add the preview images for the projects you defined in `projects.js`.
- [ ] **`static/lab/`**: Add the preview images for the experiments defined in `lab.js`.

## 5. 3D Models & Scene (Blender)
*(Located in the `resources/` folder. You will need [Blender](https://www.blender.org/) to edit these and re-export the GLTF/GLB models to the `static/` folder.)*
- [ ] **`resources/models/bruno-sudo.blend1`**: This is the main character. You'll likely want to create/swap this with a model of yourself or a car/object!
- [ ] **`resources/folio-2025.blend1`**: The main world file. Modify the terrain, remove/add buildings, reposition interactable areas.
- [ ] **`resources/textures/`**: Update/re-bake any textures that have specific lettering or branding.

## 6. Advanced Code Customization
- [ ] **`sources/Game/Title.js`**: Usually handles the intro/title scene text.
- [ ] **`sources/Game/InteractivePoints.js`**: If you rename/move 3D points in Blender, you may need to update references here or in their respective mapping files.
- [ ] **`sources/Game/Player.js` & `sources/Game/PhysicalVehicle.js`**: Tweak these if you want your character to move faster, jump higher, or change the physics of the vehicle.
