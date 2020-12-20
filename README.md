# Downloader

[![License: GNU Affero General Public license version 3](https://img.shields.io/badge/License-AGPLv3-blue.svg)](https://opensource.org/licenses/agpl-3.0)

A simple Downloader for Swift published under the GNU Affero General Public license.

Usage: 

```Swift
// URL to download
let myurl = URL(...)
// Create a Downloader instance
let downloader = Downloader()
// Register the delegate to get informed about changes.
downloader.delegate = self
// Create multiple DownloadTasks
let task1 = DownloadTask(dID: "mytaskid", source: myurl, destination: "/Path/To/Destination/file", description: "My task description")
// Start the download process
downloader.start(task1)
```
