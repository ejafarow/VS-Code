## Extensions

##YourCopyableTextblock
- Beautify css/sass/scss/less
- C/C++
- C/C++ Extension Pack
- C/C++ Themes
- CMake
- CMake Tools
- Code Runner
- Code Spell Checker
- CodeSnap
- CSS Peek
- Dev Containers
- Docker
- ES7+ React/Redux/React-Native snippets
- ESLint
- FontSize Shortcuts
- HTML CSS Support
- IntelliSense for CSS class names in HTML
- JavaScript (ES6) code snippets
- Live Server
- Material Icon Theme
- open in browser
- Paste JSON as Code
- Pretty TypeScript Errors
- Theme - Oceanic Next
- vscode-icons

let blocks = document.querySelectorAll("pre");

blocks.forEach((block) => {
    if (!navigator.clipboard) {
        return;
    }

    let button = document.createElement("button");
    button.className = "button-copy-code";
    button.innerHTML = copyIcon;
    block.appendChild(button);

    button.addEventListener("click", async () => {
        await copyCode(block);
    });
});

