# Documents and downloads

Organize non-image downloadable files by the page they belong to:

- `blog/<post-slug>/<filename.ext>`
- `tutorials/<course>/<day-or-lesson>/<filename.ext>`
- `projects/<project-slug>/<filename.ext>`
- `shared/<filename.ext>` for files reused across pages.

These folders can contain PDFs, text files, source archives, slides, spreadsheets, diagrams, or other downloadable non-image formats. Put displayed images under `assets/images/` instead. Use stable, descriptive filenames and a Jekyll link such as `[Download file]({{ "/assets/documents/projects/example/filename.ext" | relative_url }})`. Never publish credentials or private data.
