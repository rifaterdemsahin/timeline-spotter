# Timeline Spotter - Usage Guide

## Quick Start

1. Open `index.html` in your web browser
2. Start by entering your video script or notes
3. Configure your timeline length
4. Upload subtitle and artifact files (optional)
5. Search for artifacts and place them on the timeline

## Step-by-Step Guide

### 1. Script & Notes

**Purpose**: Store your video script, production notes, or keywords that will be used for artifact search.

**How to use**:
- Enter your script in the text area
- Click "💾 Save Script" to store it in cookies
- Click "📂 Load Script" to reload saved script
- The script is automatically loaded when you revisit the page

**Example**:
```
Video intro with logo animation at 0:00
Main content from 0:10 to 4:30
Background music throughout
Add lower thirds for speaker names
Transition effects at key moments
Outro with call-to-action at 4:45
```

### 2. Timeline Configuration

**Purpose**: Define the length and time unit of your video editor timeline.

**Settings**:
- **Timeline Length**: Enter duration in the selected unit (default: 300 seconds)
- **Time Unit**: Choose between:
  - Seconds (default)
  - Frames (30fps)
  - Timecode

**How to use**:
1. Enter your video's total duration
2. Select the appropriate time unit
3. Click "🔄 Update Timeline" to apply changes
4. The timeline visualization will update to match your settings

### 3. Upload Files

#### Subtitle Files

**Supported formats**: `.srt`, `.vtt`, `.txt`

**Why upload subtitles?**
- Provides accurate timestamps for content
- Improves artifact location estimation
- Enables precise keyword matching

**Example subtitle format (.srt)**:
```
1
00:00:00,000 --> 00:00:03,000
Welcome to our tutorial

2
00:00:03,500 --> 00:00:07,000
Today we'll learn about video editing
```

#### Artifact Lists

**Supported formats**: `.txt`, `.json`, `.csv`

**Plain text format** (one artifact per line):
```
Intro Logo
Opening Title
Background Music
Main Transition
Lower Third Text
```

**CSV format** (with metadata):
```csv
name,type,keywords
Intro Logo,graphic,intro opening logo branding
Background Music,audio,music soundtrack background
Main Transition,effect,transition wipe fade
```

**JSON format**:
```json
[
  {
    "name": "Intro Logo",
    "type": "graphic",
    "keywords": "intro opening logo"
  },
  {
    "name": "Background Music",
    "type": "audio",
    "keywords": "music soundtrack"
  }
]
```

### 4. Search Artifacts

**Purpose**: Find optimal locations for your artifacts based on script, subtitles, and uploaded lists.

**How the search works**:
1. Searches through your script for the keyword
2. Scans subtitle timecodes for matches
3. Checks artifact lists for matching names/keywords
4. Returns estimated positions with confidence levels

**Search tips**:
- Use specific keywords (e.g., "intro", "transition", "music cue")
- Try variations (e.g., "opening" vs "intro")
- Search for speaker names if using lower thirds
- Use generic terms to find categories of artifacts

**Results include**:
- **Source**: Where the match was found (Script/Subtitle/Artifact List)
- **Position**: Estimated location as percentage of timeline
- **Time**: Timecode (if available from subtitles)
- **Confidence**: High (direct match) or Medium (estimated)

**Actions**:
- Click "Add to Timeline" to place a specific result
- Click "📍 Place All on Timeline" to automatically distribute all artifacts from your uploaded list

### 5. Timeline Preview

**Features**:
- Visual representation of your timeline
- Time markers at 10% intervals
- Colored markers for placed artifacts
- Hover over markers to see artifact names and times

**Artifact Management**:
- Click on any marker to view details
- Click the × button to remove an artifact
- Artifacts are displayed below the timeline with their positions

### 6. Cookie Management

**All data is automatically saved in browser cookies**, including:
- Script content
- Timeline configuration
- Uploaded subtitles
- Artifact lists
- Placed artifacts

**View Cookies**:
- Click "👁️ View All Cookies" to see stored data
- Each cookie shows its name and a preview of its content

**Delete Options**:
- Click "Delete" next to any cookie to remove it individually
- Click "🗑️ Clear All Cookies" to delete everything (requires confirmation)

**Export/Import**:
- **Export**: Download all your data as a JSON file for backup
- **Import**: Upload a previously exported file to restore your work

## Advanced Tips

### Organizing Your Workflow

1. **Start with Script**: Enter your complete script first for best results
2. **Add Subtitles**: Upload accurate subtitles if available
3. **Upload Artifacts**: Use CSV format to include keywords and metadata
4. **Search Strategically**: Search for major sections first (intro, main, outro)
5. **Fine-tune**: Manually adjust artifact positions as needed
6. **Export Regularly**: Save your work before making major changes

### Keyboard Shortcuts

- Tab: Navigate between fields
- Enter: Submit forms (save script, search)
- Escape: Close modals

### Best Practices

1. **Use Consistent Naming**: Keep artifact names consistent with your script
2. **Include Keywords**: Add relevant keywords to CSV files for better matching
3. **Backup Often**: Use the export feature to save your configuration
4. **Test Searches**: Try different search terms to find optimal placements
5. **Review Results**: Check confidence levels and adjust low-confidence placements

### Troubleshooting

**Script not loading?**
- Check if cookies are enabled in your browser
- Clear all cookies and start fresh
- Try using the Export/Import feature as an alternative

**Search returns no results?**
- Verify your search term appears in the script or subtitles
- Check that files were uploaded successfully
- Try more general keywords

**Timeline not updating?**
- Click "🔄 Update Timeline" after changing length
- Refresh the page if issues persist
- Check the browser console for errors

**Artifacts not appearing?**
- Ensure you clicked "Add to Timeline" or "Place All"
- Verify the timeline length is set correctly
- Check that cookies are enabled

## Browser Requirements

- Modern browser (Chrome, Firefox, Safari, Edge)
- JavaScript enabled
- Cookies enabled
- File API support

## Data Privacy

- All data stays in your browser
- No server-side storage or tracking
- You control all data through cookie management
- Use Export/Import for data portability

## Tips for Video Editors

### For Premiere Pro Users
- Use seconds as your time unit
- Export your markers as CSV before importing
- Match your timeline length to sequence duration

### For Final Cut Pro Users
- Consider using timecode format
- Export subtitle track for accurate timing
- Use keywords that match your clip names

### For DaVinci Resolve Users
- Seconds work well for most projects
- Export EDL markers as artifact lists
- Include color coding keywords in CSV

## Example Workflow

1. **Preparation** (5 minutes)
   - Write/paste your video script
   - Set timeline length (e.g., 300 seconds for 5-minute video)
   - Upload subtitle file from your NLE

2. **Artifact Planning** (10 minutes)
   - Create artifact list (intro, logo, transitions, effects)
   - Upload as CSV with keywords
   - Review automatic placement

3. **Search & Refine** (15 minutes)
   - Search for "intro" → place intro elements
   - Search for "transition" → place transition effects
   - Search for speaker names → place lower thirds
   - Manual adjustments as needed

4. **Export & Implement** (5 minutes)
   - Export configuration as JSON backup
   - Use timeline as reference in your NLE
   - Import artifacts at specified positions

## Support & Resources

For questions, issues, or feature requests, please open an issue on GitHub.

Happy editing! 🎬
