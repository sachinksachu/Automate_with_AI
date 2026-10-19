Added HTML validation setup with GitHub Actions, config files, and package dependencies.
Removed the `alt` text attribute from the newsletter banner image in `index.html`, causing an accessibility issue.

* **`index.html`**:
  * **Issue:** The `<img>` tag is missing the `alt` attribute, which is required for screen readers and accessibility.
  * **Fix:** Restore the `alt` attribute or mark it decorative (`alt=""`).
    ```html
    <img src="banner.jpg" alt="Newsletter banner">
    ```

* **`.github/workflows/checks.yml`**:
  * **Issue:** Missing trailing newline at the end of the file.
  * **Fix:** Add a newline at the end of the file to adhere to standard POSIX formatting.
