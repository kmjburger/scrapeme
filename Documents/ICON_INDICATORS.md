# 🎨 Icon Status Indicators

StepGallery now shows **animated icon badges** to indicate what the extension is doing in real-time!

## Icon States

### 🔵 **Paginating** (Blue Spinning Circle)
- **What it shows**: `○ ◔ ◑ ◕ ● ◕ ◑ ◔` (animated)
- **Color**: Blue (#2196F3)
- **Meaning**: Extension is navigating to the next page
- **When you see it**: After current page downloads complete, while waiting to load next page

### 📊 **Downloading** (Green Percentage)
- **What it shows**: `45%` or download count
- **Color**: Green (#4CAF50)
- **Meaning**: Images are actively downloading
- **When you see it**: During batch image downloads from current page

### ⏳ **Waiting** (Orange Hourglass)
- **What it shows**: `⏳` or `5s` (countdown)
- **Color**: Orange (#FF9800)
- **Meaning**: Extension is waiting between actions (adaptive delay)
- **When you see it**: Between page transitions, during adaptive timing delays

### ⏸️ **Paused** (Red Pause Symbol)
- **What it shows**: `⏸`
- **Color**: Red (#FF5722)
- **Meaning**: Pagination is paused (waiting for you to resume)
- **When you see it**: After you click "Pause" button

### ✓ **Complete** (Green Checkmark)
- **What it shows**: `✓`
- **Color**: Green (#4CAF50)
- **Meaning**: Operation completed successfully
- **When you see it**: After all pages processed or download complete
- **Note**: Auto-clears after 3 seconds

### ⚠️ **Error** (Red Exclamation)
- **What it shows**: `!`
- **Color**: Red (#F44336)
- **Meaning**: An error occurred
- **When you see it**: If something goes wrong during pagination/download

### ⚪ **Idle** (No Badge)
- **What it shows**: (empty - no badge)
- **Meaning**: Extension is ready but not actively working
- **When you see it**: Default state, before starting or after completing

## How to See the Icon

Look at the **Chrome extension icon** in your toolbar (top-right of browser):
- The icon shows `icons/icon16.png` by default
- The **badge** (small text overlay) changes based on activity
- Badge appears in the **bottom-right corner** of the icon

## Example Flow

```
1. You click "Start Pagination"
   → Icon shows: ○ ◔ ◑ ◕ (blue, spinning)

2. First page images start downloading
   → Icon shows: 15% (green)

3. Downloads complete, waiting for next page
   → Icon shows: ⏳ (orange)

4. Next page loads, downloading again
   → Icon shows: 47% (green)

5. All pages complete
   → Icon shows: ✓ (green, for 3 seconds)
   → Icon returns to: (no badge)
```

## Benefits

✨ **At-a-glance status**: Know what the extension is doing without opening the dashboard  
⏱️ **Better UX**: No more wondering "is it stuck or just waiting?"  
🎯 **Visual feedback**: See progress percentages during downloads  
🔄 **Activity awareness**: Know when pagination is active vs idle
