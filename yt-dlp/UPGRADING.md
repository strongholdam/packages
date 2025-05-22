# Upgrading YT-DLP

This guide outlines the steps to update YT-DLP. Follow these instructions to ensure that the server has the latest version of YT-DLP.

## 1. Check for the Latest Version

Visit the [YT-DLP Releases](https://github.com/yt-dlp/yt-dlp/releases) page to determine the most recent version available.

## 2. Download and Publish the New Version

If a new version is available:

- **Download:** Obtain the latest release.
- **Copy:** the downloaded version to replace the `current` file in the repository.
- **Publish:** Commit the new version to the shared repository.

## 3. Update on the Server

Log in to the server and run the following commands to update YT-DLP:

```bash
curl -L https://github.com/strongholdam/packages/raw/refs/heads/main/yt-dlp/current -o /usr/local/bin/yt-dlp
sudo chmod a+rx /usr/local/bin/yt-dlp
```

## 4. Verify the Update

Run the command below to ensure that YT-DLP is up-to-date:

```bash
yt-dlp --version
```

By following these steps, you can maintain an updated version of YT-DLP on the server.
