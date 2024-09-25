# URL to Markdown Collector

A minimalistic Firefox extension that allows you to collect URLs, convert the content of each page into Markdown and copy it to your clipboard effortlessly.

## Features

- **Quick Save:** Use a keyboard shortcut to save the current page's URL and convert its content to Markdown.
- **Markdown Collection:** Access a centralized page to view and manage all your saved URLs and their Markdown content.
- **Editable Content:** Edit Markdown directly within the collection page. Changes are saved automatically upon editing.
- **Export Markdown:** Concatenate and copy all collected Markdown content to your clipboard.

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/url-to-markdown-collector.git
   ```

2. **Load the Extension in Firefox:**
   - Open Firefox and navigate to `about:debugging#/runtime/this-firefox`.
   - Click on **"Load Temporary Add-on..."**.
   - Select the `manifest.json` file from the cloned repository.

## Usage

1. **Save a Page:**

   - Press the keyboard shortcut `Alt+I` to save the current page's URL and convert its content to Markdown
   - or click the extension icon and select **"Copy as Markdown"**, which will copy the contents of the current page to your clipboard and save it to the collection.

2. **View and Manage Collected Markdown:**

   - Press the keyboard shortcut `Alt+C` or click the extension icon and select **"Open Collection"** to view all saved URLs and their Markdown content.
   - In the collection page, you can:
     - **Edit Markdown:** Click inside a Markdown box to edit its content. Changes are saved automatically.
     - **Copy Markdown:** Select desired entries and click the **"Copy"** button to copy the concatenated Markdown to your clipboard.
     - **Delete Entries:** Select entries and click the **"Delete"** button to remove them from your collection.
     - **Update Markdown:** Select entries and click the **"Update"** button to refresh the Markdown content from the source page. This will show the diff of the old and new markdown content, which you can accept or reject **at the bottom of the diff popup**.

3. **Copy Markdown:**
   - After ensuring all Markdown content is fully scraped (this is generally very fast), use the **"Copy"** button to copy all Markdown data, including URLs and titles, separated by XML tags.

## Keyboard Shortcuts

- **Save Current URL and Convert to Markdown:** `Alt+I`
- **Open Markdown Collection Page:** `Alt+C`

_You can customize these shortcuts in the Firefox Add-ons settings._

## Contributing

Contributions are welcome! Whether it's reporting bugs, suggesting features, or submitting pull requests, your help is appreciated.

1. **Fork the Repository**
2. **Create a New Branch:**
   ```bash
   git checkout -b feature/YourFeature
   ```
3. **Commit Your Changes:**
   ```bash
   git commit -m "Add some feature"
   ```
4. **Push to the Branch:**
   ```bash
   git push origin feature/YourFeature
   ```
5. **Open a Pull Request**

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- [Turndown](https://github.com/domchristie/turndown) for HTML to Markdown conversion.
- [JsDiff](https://github.com/kpdecker/jsdiff) for showing differences between Markdown texts.
