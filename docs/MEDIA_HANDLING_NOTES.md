# Media Handling Notes

These notes capture the edge cases that should stay visible during Gallery development.

## Cases to retest

- Albums containing only videos.
- Albums containing hidden or unsupported files.
- Very large images that need downsampling.
- Media files added while the app is open.
- Storage permission changes from Android settings.

## Expected behavior

The UI should stay responsive while thumbnails load, and unsupported files should fail quietly with a clear empty or unavailable state.
