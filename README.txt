All Mobile Video v48

MICROSOFT 403 FIX

The previous version's Entra app registration had Files.ReadWrite.All added,
but the web app itself was still requesting only Files.ReadWrite.

v48 now requests:
- User.Read
- Files.ReadWrite
- Files.ReadWrite.All

It also:
- Forces a fresh Microsoft consent screen.
- Uses a new token cache key so the old token cannot be reused.
- Keeps the existing GitHub Pages redirect URI and JOBS folder configuration.

After uploading v48 to GitHub:
1. Open the live GitHub Pages site.
2. Refresh the page.
3. Click CONNECT ONEDRIVE.
4. Microsoft should show the permission consent screen again.
5. Accept it.
6. The app will return to GitHub Pages and retry the JOBS folder.

If a 403 still occurs after v48, the likely remaining issue is that the
signed-in Microsoft user does not itself have Edit permission to the shared
JOBS folder, or a tenant policy is restricting Graph access.
