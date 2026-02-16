# 🎬 Timeline Spotter

Find location for your artifacts on a non-linear video editor with intelligent search and estimation.
> https://rifaterdemsahin.github.io/timeline-spotter/

## Features

### 🎯 Core Functionality
- **Script Input & Storage**: Enter and save video scripts, notes, or keywords in browser cookies
- **Timeline Configuration**: Set your video timeline length in seconds, frames, or timecode format
- **Subtitle Upload**: Upload `.srt` or `.vtt` subtitle files to improve artifact location estimates
- **Artifact List Management**: Upload artifact lists in `.txt`, `.json`, or `.csv` formats
- **Intelligent Search**: Search for artifacts and get estimated locations on your timeline
- **Visual Timeline**: Interactive timeline preview showing all placed artifacts
- **Cookie Management**: Complete control over saved data with individual or bulk delete options

### 🔍 Search & Estimation
The search function analyzes multiple sources to estimate artifact locations:
- Searches through your script/notes
- Scans subtitle timecodes for relevant keywords
- Matches against uploaded artifact lists
- Provides confidence levels (High/Medium) for each estimate

### 💾 Data Persistence
All data is automatically saved in browser cookies:
- Script content
- Timeline configuration
- Uploaded subtitles
- Artifact lists
- Placed artifacts on timeline

### 📥 Import/Export
- Export all your data to a JSON file for backup
- Import previously exported data to restore your work
- Share configurations across projects

## Usage

### Getting Started
1. Open `index.html` in your web browser
2. Enter your timeline length (e.g., 300 seconds for a 5-minute video)
3. (Optional) Enter script notes in the Script & Notes section
4. (Optional) Upload subtitle and artifact files for better estimates

### Searching for Artifacts
1. Enter a search term (e.g., "intro", "transition", "logo")
2. Click "🔍 Find Locations" to search across all sources
3. Review the estimated positions and confidence levels
4. Click "Add to Timeline" to place artifacts on your timeline

### Managing Artifacts
- Click on any artifact marker on the timeline to view details
- Use "📍 Place All on Timeline" to automatically distribute all uploaded artifacts
- Remove individual artifacts using the × button
- Export your complete timeline configuration for later use

### Cookie Management
- Click "👁️ View All Cookies" to see all stored data
- Delete individual cookies for selective data removal
- Use "🗑️ Clear All Cookies" to reset everything
- Export data before clearing to create a backup

## Sample Files

The repository includes sample files for testing:
- `sample-artifacts.txt` - Plain text list of common video artifacts
- `sample-artifacts.csv` - CSV format with artifact metadata
- `sample-subtitles.srt` - Sample subtitle file with timestamps

## Technical Details

### Supported File Formats
- **Subtitles**: `.srt`, `.vtt`, `.txt`
- **Artifacts**: `.txt`, `.json`, `.csv`

### Cookie Storage
All cookies are stored with a 365-day expiration and include:
- `timeline_script` - User's script/notes
- `timeline_length` - Timeline duration
- `timeline_unit` - Time unit (seconds/frames/timecode)
- `timeline_data` - Complete timeline with artifacts
- `timeline_subtitles` - Parsed subtitle data
- `timeline_artifacts` - Uploaded artifact list

### Browser Compatibility
Works in all modern browsers that support:
- ES6 JavaScript
- File API
- Cookie storage
- CSS Grid

## Tips for Best Results

1. **Upload Subtitles First**: Subtitle files provide the most accurate timestamps for artifact placement
2. **Use Descriptive Keywords**: When searching, use terms that appear in your subtitles or script
3. **Regular Exports**: Export your data periodically to avoid losing work
4. **Organized Artifact Lists**: Use CSV format with keywords for better search matches
5. **Script Notes**: Add detailed notes about where artifacts should appear

## Privacy & Security

- All data is stored locally in your browser cookies
- No data is sent to external servers
- You have complete control over your data
- Use export/import to backup and transfer data safely

## License

Open source - feel free to use and modify for your projects!
