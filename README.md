# sp-publish-js action

This action publishes a folder to a Sharepoint library

## Inputs

## `output_folder`

**Required** Folder to publish

## `site_url`

**Required** URL of the Sharepoint site

## `sharepoint_user`

**Required** Sharepoint username

## `sharepoint_password`

**Required** Sharepoint password

## `library_folder`

**Required** Sharepoint folder to publish to

## Example usage
```
-name: Publish to Sharepoint
 uses: jhkenney/sp-publish-js@v1
 with:
  output_folder: 'appName\bin\Release'
  site_url: 'https://example.sharepoint.com/sites/documents'
  sharepoint_user: ${{ secrets.SHAREPOINT_USER }}
  sharepoint_password: ${{ secrets.SHAREPOINT_PASSWORD }}
  library_folder: Software/AppName
```