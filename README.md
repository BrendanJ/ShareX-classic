<h1 align="center">ShareX Classic</h1>
<h3 align="center">Screen capture, file sharing and productivity tool</h3>
<p align="center"><b>THIS IS AN UNOFFICIAL FORK - NOT AFFILIATED WITH THE SHAREX TEAM</b></p>
<br>
<div align="center">
  <a href="https://github.com/BrendanJ/ShareX-classic/actions/workflows/build.yml"><img src="https://img.shields.io/github/actions/workflow/status/BrendanJ/ShareX-classic/build.yml?branch=classic&label=Build&cacheSeconds=3600" alt="GitHub Workflow Status"/></a>
  <a href="./LICENSE.txt"><img src="https://img.shields.io/github/license/BrendanJ/ShareX-classic?label=License&color=brightgreen&cacheSeconds=3600" alt="License"/></a>
  <a href="https://github.com/BrendanJ/ShareX-classic/releases/latest"><img src="https://img.shields.io/github/v/release/BrendanJ/ShareX-classic?label=Release&color=brightgreen&cacheSeconds=3600" alt="Release"/></a>
</div>
<br>

ShareX Classic continues [ShareX](https://github.com/ShareX/ShareX) from version 21.0.0, the last release before the version 22 interface redesign. The goal is a simple, clean, consistent and reliable ShareX with the interface longtime users know.

## Differences from ShareX 21.0.0
* **Classic image editor only.** Avalonia has been removed entirely. The WinForms image editor is the only editor, so there is no editor selection prompt. The Background remover and Image comparer tools, which were added in 21.0.0 and depended on Avalonia, are not included.
* **.NET 10.** Built on .NET 10 (LTS), because .NET 9 reaches end of support on November 10, 2026.
* **Updates come from this repository.** The built-in update checker looks at ShareX Classic releases, never at upstream ShareX.
* **Drop-in replacement.** ShareX Classic uses the same install folder, settings folder (`Documents\ShareX`), history and single-instance lock as ShareX, so it picks up your existing configuration. Run only one of ShareX or ShareX Classic at a time.

## Building
1. Install the [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or Visual Studio 2026 with the .NET desktop workload.
2. Open `ShareX.sln` and build the `Release` configuration for `x64`.

Some built-in uploaders, such as Imgur, Dropbox, Google Drive and OneDrive, need API keys that are not part of the source code. Without them, those uploaders will not work in your build. Custom uploaders and uploaders that take your own credentials are not affected.

## Credits
ShareX Classic is built on the work of the ShareX Team and its contributors. It is distributed under the same [GNU General Public License v3.0](./LICENSE.txt).

## Documentation
Most of the ShareX documentation still applies:
* Image effects: https://getsharex.com/image-effects
* Actions: https://getsharex.com/actions
* Keybinds: https://getsharex.com/docs/keybinds
* Scrolling screenshot: https://getsharex.com/docs/scrolling-screenshot
* Command line arguments: https://getsharex.com/docs/command-line-arguments
* OCR: https://getsharex.com/docs/ocr
* Custom uploader: https://getsharex.com/docs/custom-uploader
* Amazon S3 guide: https://getsharex.com/docs/amazon-s3
* Google Cloud Storage guide: https://getsharex.com/docs/google-cloud-storage
* Cloudflare R2 guide: https://getsharex.com/docs/cloudflare-r2
