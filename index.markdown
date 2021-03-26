---
title: File Renaming in Bulk
layout: default
has_children: true
nav_order: 1
---

# File Renaming in Bulk

### Tools in Use:
- bash
- LibreOffice Calc

### Method:
1. n bash, create a list of the filenames of the archival collection you are processing (paths included); redirect to write to a text file.
2. In LibreOffice Calc, copy/paste the contents of that text file into Column A, and into Column B too.
3. Make Column A header "original filename". Make Column B header "new filename"
4. Select all of Column B. Using Find + Replace with regex, make changes you want to any filenames (replacing `$` with `USD`, for example)
5. Save the file as UTF-8 CSV type and call it something like `filename_changes.csv`
6. After you've finished making new filenames and folder names as needed, save and close the new UTF-8 CSV `filename_changes.csv`, making sure to change the delimiter to be a pipe (`|`) rather than a comma.
7. In a bash terminal, from the directory containing your collection:  
`sed 's/"//g' filename_changes.csv | while IFS="\|" read orig new; do mv "$orig" "$new"; done`

*Notice that the IFS is set to the pipe, not a comma.*  

As a result, you have new filenames across your collection per your decisions, which was documented alongside the original filenames in the CSV file. Include this administrative CSV file in submission documentation in the AIP.

### Alternative method: a PowerShell One-Liner!
*please, be very careful*

Replace spaces with underscores through the filename and the full path...


`get-childItem . | foreach {rename-item $_ $_.name.replace(" ", "_")}`

Because this is an aggressive approach, this method is best for truly bulk tasks, like for *deleting* or *replacing* all spaces from folder and file paths. It's not great when it comes to replacements like `$` to `USD`.






