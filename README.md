# ChatGPT Search Engine

Adds ChatGPT as a search engine to your Firefox browser. In the URL bar, you can simply type `@chatgpt your_query` to access ChatGPT directly.

I am also developing another great extension, a multi-search engine tool currently in development. Take a look at it [here](https://github.com/atahabaki/smart-search). I highly recommend it.

If you want to follow what I'm currently working on and developing, stay tuned!

## Screenshots

![@chatgpt search](./show.png)

## How It Works

Firefox utilizes the `chrome_settings_overrides.search_provider` in the `manifest.json` file to add custom search engines to the omnibox. This extension leverages that feature to integrate ChatGPT as a searchable option.

For more details, please refer to the [MDN documentation](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/manifest.json/chrome_settings_overrides).

## Installation

1. **Download the Extension**:
   - Clone the repository using `git clone https://github.com/yourusername/firefox-chatgpt-addon.git` or download the ZIP file and extract it.

2. **Open Firefox**:
   - Navigate to `about:debugging` in the Firefox address bar.

3. **Load the Add-on**:
   - Click on “Load Temporary Add-on” and select the `manifest.json` file from the extracted folder.

4. **Test the Extension**:
   - Open the Firefox address bar and type `@chatgpt Your question`. This should open the ChatGPT webpage where you can manually enter your query.

## Notes

- **Functionality**: Since ChatGPT does not support direct search URLs, the search query redirects you to the ChatGPT webpage, where you need to input your query manually. This differs from traditional search engines that display results directly.

- **Alternative Approaches**:
  - **Custom Web Application**: You can create a custom web application using the OpenAI API to handle search queries and display results. This requires backend development and an OpenAI API key.
  - **Integration with Existing Tools**: If you use tools integrated with the OpenAI API, you can incorporate them into your workflow instead of creating a new search engine.

- **Security and Privacy**: Ensure that you do not transmit sensitive information through search queries and comply with OpenAI's privacy policies when using the API.

## License

This project is licensed under the [MIT License](LICENSE).

## Contributions

Contributions are welcome! Please open an issue or submit a pull request if you have any improvements or suggestions.

## Author

- **Fabian Druschke**

