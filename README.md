<img width="382" alt="Screen Shot 2020-11-26 at 2 15 36 AM" src="https://user-images.githubusercontent.com/10296053/100324905-7c770080-2f8d-11eb-8521-fa3b173156b7.png">

# Mac: Share to Nextcloud
A Quick Action for macOS, using the native Quick Actions. You can right-click files and run this. It will upload the file to Nextcloud, create a Share link, and copy the Share link to your Clipboard. It will send a Notification when the link is ready. All without installing any apps.

<img width="533" alt="Right click Quick Action" src="https://user-images.githubusercontent.com/10296053/100324597-18543c80-2f8d-11eb-8d26-6300bb887a02.png">

## How to download and use
You can download this repository to your Mac, or use the latest in [releases](https://github.com/melyux/mac-share-to-nextcloud/releases).

You then must enter some details about your Nextcloud situation before using it. To do this, right-click the Workflow file → Open With → Automator (NOT Automator Installer, which is the default). In the Automator window, fill out the details in the requested "Get Specified Text" actions:

* **Host**: the URL of your Nextcloud instance, without the protocol (e.g. nextcloud.domain.me)
* **Folder**: an existing folder in your Nextcloud instance to upload the file to (e.g. Shortcuts)
* **Username**: your Nextcloud username
* **Token**: your app-specific password created just for this; to create one, go to Nextcloud → Settings → Devices & sessions and create a new app password

Do File → Save (or Command + S) to save.

Now double click the Workflow file to install it to your Mac.

To edit any of these parameters in the future, find the file in `~/Library/Services/Share through Nextcloud.workflow` to edit it in the same way using Automator.
