# **Customizing VS Code with Custom CSS & JS**

Enhance your Visual Studio Code experience by injecting custom CSS and JavaScript. Follow this guide to set up and personalize your VS Code environment.

**NOTE:** Please take time to read the short documentation of **"Custom CSS and JS Loader"** for some useful tips for various operating systems to avoid issues regarding the changes not taking effect.

## 🚀 **Installation Guide**

1️⃣. Install Required Extension

    Install the Custom CSS and JS Loader extension in VS Code.

2️⃣. Configure VS Code Settings

    1. Open VS Code and navigate to settings.json.

    2. Copy and paste the following snippet into your settings.json file:

```
"vscode_custom_css.imports": [
    // Absolute file paths for your css/js files
    // For Mac or Linux
    // "file:///Users/your-user-name/custom-vscode.css",
    // "file:///Users/your-user-name/custom-vscode-script.js"

    // For Windows
    // "file:///C:/path-of-custom-css/custom-vscode.css",
    // "file:///C:/path-of-custom-css/custom-vscode-script.js"
],
```
     ⚠️ ( it will overwrite your settings )


3️⃣. You might need to take ownership of the CSS/JS files you made or run VS Code with admin privileges on certain operating system:
```
Mac and Linux users
The extension would NOT work if Visual Studio Code cannot modify itself. The cases include:

Code files being read-only, like on a read-only file system or,
Code is not started with the permissions to modify itself.
You need to claim ownership on Visual Studio Code's installation directory, by running this command:

Note: Replace /usr/share/code where your VS Code is installed.
sudo chown -R your-user-name /usr/share/code
```
4️⃣. Enable Custom CSS & JS

    1. Open Command Palette (Ctrl + Shift + P or Cmd + Shift + P on Mac).
    2. Search for and select "Enable Custom CSS and JS".

5️⃣. Customize the css or js from this repo to make it look the way you want to, or even better, explore areas of VS Code that you want to customize. 

        from vs code choose help --> Toggle Developers Tools --> choose what ever you want and then add the style to your style sheet with your Customization. 

6️⃣. After making some changes, reload the extension (Reload Custom CSS and JS) from VS Code's command dialog.


## 🎨 **Customization Ideas**

- Change editor fonts and colors
- Customize sidebar, status bar, and tabs
- Modify animations and transitions
- Add custom JavaScript functionality

## 🛠 **Troubleshooting**

- If changes don’t take effect, restart VS Code.
- Ensure file paths in settings.json are correct.
- Run VS Code as an administrator (Windows) or adjust permissions (Mac/Linux).
