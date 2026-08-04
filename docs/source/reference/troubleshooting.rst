============================================
Troubleshooting & Frequently Asked Questions
============================================

Find solutions to common setup and configuration issues encountered when using the MARV extension.

1. API Endpoint Errors
----------------------

**Issue:** Sidebar displays API Error: Failed to fetch tutorials.

**Solution:**
1. Check that your API URL is set exactly to https://marv.computing.edgehill.ac.uk.
2. Ensure there are no space characters or extra path suffixes at the end of the URL.
3. Click the **Refresh Icon (🔄)** at the top of the MARV sidebar.

2. VSIX Installation Fails
--------------------------

**Issue:** VS Code returns Incompatible API version or installation hangs.

**Solution:**
1. Upgrade Visual Studio Code to the latest stable release (v1.70.0+ required).
2. Restart VS Code completely before retrying **Install from VSIX...**.

3. Student ID Configuration Issues
----------------------------------

**Issue:** User icon does not appear or Student ID prompt fails to save.

**Solution:**
1. Hover over the **Available tutorials** header text in the MARV sidebar.
2. Click the rightmost **User Icon** revealed on hover.
3. Enter your numeric Student ID and press Enter.

4. Workspace Connection Warnings
--------------------------------

**Issue:** Sidebar displays No folder open in workspace (Click to open).

**Solution:**
1. Click the warning prompt in the MARV sidebar to choose a workspace directory.
2. Alternatively, open a folder via VS Code **File -> Open Folder...**.
