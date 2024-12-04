# Advanced Markdown Editor

This repository contains the **Advanced Markdown Editor**, a powerful and user-friendly editor for creating and previewing Markdown content with support for real-time updates. The editor is built using [EasyMDE](https://easymde.com/) and features a modern design, rich formatting tools, and a live preview pane.

## Features

- **Markdown Editing**: Write Markdown content easily using an intuitive interface.
- **Rich Toolbar**: Includes tools for bold, italic, headings, lists, quotes, code blocks, and more.
- **Live Preview**: See real-time updates of your rendered Markdown.
- **Autosave**: Automatically saves your work to local storage every second.
- **Responsive Design**: Optimized for all screen sizes.
- **Emoji Support**: Write emojis directly using standard emoji syntax (e.g., `:smile:`).

## Live Demo

Check out the live version of the Advanced Markdown Editor here:

[Advanced Markdown Editor Live Demo](https://jawadabbasi14.github.io/markdown-editor/)

## Usage

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/JawadAbbasi14/markdown-editor.git
   ```
2. Navigate to the project directory:

   ```bash
   cd markdown-editor
   ```
3. Open `index.html` in your browser to start using the editor.

### Adding Emoji Support

To enhance your Markdown editor with emojis, include emoji libraries like [Twemoji](https://github.com/twitter/twemoji) or [emojione](https://github.com/emojione/emojione):

#### Example Integration:

1. Add Twemoji JavaScript to your `index.html`:

   ```html
   <script src="https://cdnjs.cloudflare.com/ajax/libs/twemoji/14.0.2/twemoji.min.js"></script>
   <script>
       document.addEventListener('DOMContentLoaded', () => {
           const previewContent = document.getElementById('preview-content');
           const observer = new MutationObserver(() => {
               twemoji.parse(previewContent);
           });
           observer.observe(previewContent, { childList: true, subtree: true });
       });
   </script>
   ```
2. Write emojis in Markdown using `:emoji-name:` syntax (e.g., `:smile:`).

## File Structure

```plaintext
markdown-editor/
├── index.html       # Main HTML file
├── styles.css       # Custom styles
├── script.js        # Editor logic and functionality
└── README.md        # Project documentation (this file)
```

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve this project.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact

Created by **Jawad Abbasi**.

- GitHub: [JawadAbbasi14](https://github.com/JawadAbbasi14)
- Live Project: [Markdown Editor Live Demo](https://jawadabbasi14.github.io/markdown-editor/)
