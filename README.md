# 🤖 Auto Mode

**One-Click Automation** for complete translation workflow

## Features
- ⚡ **3-Phase Automation** - Reduces 8-10 manual steps to just 3
- 🛡️ **Symbol Validation** - Automatic 𓁳 and \n count checking
- 💾 **State Persistence** - Pause and resume anytime
- 📊 **Real-time Progress** - Live tracking of all operations
- 🔄 **Smart Error Handling** - Guided fixes with detailed instructions
- 📁 **Auto Backup** - All important files backed up automatically

## Quick Start
1. Select folders (En Old.V, Translate Old.V, EN New.V)
2. Select Dict.txt file
3. Click "Start Auto" → Follow confirmation dialogs
4. Done! Get your translated mod in `output/`

## Time Savings
- **Manual Mode:** 30-60 minutes
- **Auto Mode:** 5-15 minutes (excludes AI translation time)
- **You Save:** 50-75% of your time!

## Workflow Overview

### Phase 1: Extract & Dict
- Extracts updated text from new game version
- Auto-extracts dictionary from text
- **You:** Review Dict.txt, click Confirm

### Phase 2: Prepare Translation
- Converts game codes to Unicode
- Removes duplicate lines (reduces translation cost)
- **You:** Translate with AI, import file, click Confirm

### Phase 3: Merge & Complete
- Restores translations to all lines
- Converts Unicode back to game codes
- Merges into game file structure
- **Result:** Ready-to-use mod!

## Symbol Validation

Auto Mode includes **automatic symbol validation** to ensure translation quality:

- **Validates:** 𓁳 (variables) and \n (line breaks) counts
- **Compares:** Translation against original
- **Detects:** Missing, extra, or misplaced symbols
- **Guides:** Shows exactly which lines need fixing
- **Ensures:** 100% accuracy before proceeding

### Example
```
✅ Correct: 3× 𓁳, 1× \n matches original
❌ Wrong:   1× 𓁳, 1× \n (system catches this!)
```

## Performance

| Files | Lines   | Processing Time |
|-------|---------|-----------------|
| 100   | 5,000   | ~1.5 minutes    |
| 500   | 25,000  | ~6 minutes      |
| 1,000 | 50,000  | ~12 minutes     |
| 2,000 | 100,000 | ~23 minutes     |

## Safety Features

- ✅ Never modifies original files
- ✅ Automatic backups at critical steps
- ✅ All intermediate files saved
- ✅ Full rollback capability
- ✅ State saved - resume anytime

## When to Use

**Auto Mode:**
- Game updates with new content
- Want speed and convenience
- First time translating
- Want error prevention

**Manual Mode (5 Tabs):**
- Need fine-grained control
- Custom workflow requirements
- Debugging specific issues
- Learning the process

## Files Generated

Auto Mode creates all necessary files in `output/`:
- Translation files (clean, unique, final)
- Mapping files (for restoration)
- Backup files (for safety)
- Error files (if validation fails)
- Complete mod folder (ready to use)

## Error Handling

If symbol validation fails:
1. System creates `Error_line.txt` with problematic lines
2. Creates `Original_Compare_Line.txt` for reference
3. Shows dialog with clear instructions
4. You fix the errors in `Error_line.txt`
5. Click Confirm → System validates again
6. Repeats until 100% correct

## Tips for Best Results

### Dict.txt
- Remove common English words
- Keep game codes: `[xxx]`, `$XXX$`, `§X`, `£xxx£`
- Review carefully before confirming

### AI Translation
Prompt template:
```
Translate from English to [Language]:
- Keep ALL 𓁳 symbols unchanged
- Keep ALL \n symbols unchanged  
- Only translate text
- Maintain line count
```

### Post-Processing
Use Tab 5 to check for:
- Remaining English text
- Encoding issues
- Misplaced symbols

## Full Documentation

For detailed information on each phase, file structure, and advanced features, see the complete documentation above.

---
```
📅 09:00 - Start
├─ Open Auto Mode
├─ Select folders and files
├─ Click "Start Auto (Phase 1)"
│
📅 09:03 - Phase 1 Complete
├─ Review Stellaris_Dict_V.4.2.4.txt
├─ Remove 20 incorrect words
├─ Click "I Confirm"
│
📅 09:06 - Click "Continue (Phase 2)"
│
📅 09:08 - Phase 2 Complete
├─ Send file to ChatGPT for translation
│
📅 10:30 - ChatGPT translation complete
├─ Click "Browse & Import"
├─ Select translated file
├─ ❌ Validation fail! 15 lines with errors
├─ Fix Error_line.txt
├─ Click "I Confirm - Fixed"
├─ ✅ Validation pass!
├─ Click "I Confirm" (Translation confirmation)
│
📅 10:35 - Click "Continue (Phase 3)"
│
📅 10:42 - Complete!
└─ Mod ready at output/Updated_Translation/
```

**Made with ❤️ for the Stellaris Modding Community**


