# This is an example build page for BioEchem⚡Builds
<img width="547" height="347" alt="Screen Shot 2025-09-06 at 2 34 48 AM" src="https://github.com/user-attachments/assets/01badfd3-68bb-44bc-ae96-c94b267e5c9e" />

### NIH 3D Print Database - Deposit Your Build
https://3d.nih.gov/<build>
### Protocols.io - Deposit Your Protocols
[protocols.io ](https://www.protocols.io/)

## Step 1: Deploy your build page:

1. **Fork** this repo into your GitHub account. The name of the new repo should be the name of your build.
2. **Clone** into local directory and open in Visual Studio Code. (make sue are signed in to you git account).
3. Install Node.js

4. **Change build name in main/vite.config.js**
   - Edit line 8.

5. **Change github page name to build name in main/package.json**
   - Edit line 3.
   ## Push Changes

6. **In Terminal Install dependencies:**
   
   ```bash
   npm install gh-pages
   ```
   ```bash
   npm audit fix
   ```
   ```bash
   npm install
   ```

8. **Check build on local server**

   ```bash
   npm run dev
   ```

9. ## Deploy
    
   ```bash
   npm run deploy
   ```

Your build should now be available on a webpage at https://${github_username}.github.io/${build_name}

## Step 2: Edit your build page:
```
build/
├── public/
│   └── lightning1.svg/
│   └── vite.svg
├── src/
│   ├── assets/
│   │   └── build.png
│   ├── components/
│   │   ├── Navbar.jsx
│   │   ├── MobileMenu.jsx
│   │   ├── LoadingScreen.jsx
│   │   └── sections/
│   │       ├── Home.jsx #Title, description
│   │       └── About.jsx #Author info, link to profiles, protocols
│   ├── index.css          
│   ├── App.jsx
│   └── main.jsx
├── package.json
├── vite.config.js
├── build_CAD.pdf
├── build_partlist.xlsx
├── index.html
└── README.md
```
1. **Replace files in /main with your CAD .pdf file named <build>_CAD.pdf and your your Part List .xlsx file named <build>_partlist.pdf**
   These files must be in local and in your git page in the /main directory.

2. **Replace image file in /main/src/assets with build.png file**

3. **Change content links for your build in main/src/components/section/Home.jsx**
   - Edit content lines 16 and 19 - Build title and description.

4. **Change links for your build in main/src/components/section/Usage.jsx**
   - Edit content in buildProtocols for your build.
   - Edit content line 25 - Build details.
   - Edit content line 53, 56 - Author info.
   - Edit lines 58 - 83 for author profile links. (Only "href=" links need to be modified. "src=" links are logos and remain unchanged.)

## Step 3: Deploy Edits:

11. ## Push changes.
12. Use ``` npm run dev ``` to check page on local server. Use ```npm run deploy``` to deploy.


## Additional Page Components

Visit https://github.com/swath1pen/bioreactor for source code to add 3D models to your page.
Render 3D .gltf scense using https://threejs.org/editor/.


## License

This project is open source and available under the [MIT License](LICENSE).
---

Happy building/coding/experimenting!
