# Video Setup Instructions

## Required Video Files

To display the video comparison on the website, you need to add video files to this `videos/` folder.

### iPhone Video
- **Preferred:** `iphone.mp4` (MP4 format, recommended for web compatibility)
- **Alternative:** `Iphone.MOV` (MOV format, may not work in all browsers)
- **Optional:** `iphone.webm` (WebM format for better compression)

### Pixel Video
- **Preferred:** `pxl.mp4` or `pixel.mp4` (MP4 format, recommended for web compatibility)
- **Optional:** `pxl.webm` or `pixel.webm` (WebM format for better compression)

## Video Format Recommendations

### Best Format: MP4 (H.264)
- **Codec:** H.264 video, AAC audio
- **Container:** MP4
- **Compatibility:** Works in all modern browsers
- **File extension:** `.mp4`

### Converting Videos

If you have videos in other formats (like MOV), you can convert them to MP4 using:

#### Using FFmpeg (Command Line)
```bash
# Convert MOV to MP4
ffmpeg -i Iphone.MOV -c:v libx264 -c:a aac -strict experimental iphone.mp4

# Convert any video to MP4
ffmpeg -i input.mov -c:v libx264 -c:a aac output.mp4
```

#### Using Online Converters
- [CloudConvert](https://cloudconvert.com/mov-to-mp4)
- [FreeConvert](https://www.freeconvert.com/mov-to-mp4)
- [Online-Convert](https://www.online-convert.com/)

#### Using Video Editing Software
- **Windows:** HandBrake (free), VLC Media Player
- **Mac:** HandBrake (free), QuickTime Player (can export as MP4)
- **Online:** Canva, Clipchamp

## File Size Recommendations

For web hosting, try to keep videos under 50MB each for faster loading:
- Use compression settings that balance quality and file size
- Consider reducing resolution if videos are very large
- 1080p (1920x1080) is usually sufficient for web playback

## Testing

After adding videos:
1. Refresh your browser
2. Navigate to the "The Failures" section
3. Click on the "Critical Media & Hardware Failure" tab
4. Videos should automatically load and play

If videos don't appear:
- Check that file names match exactly (case-sensitive on some servers)
- Verify file permissions allow reading
- Check browser console for error messages
- Ensure videos are in the `videos/` folder (not a subfolder)

## Deployment Notes

When deploying to GitHub Pages, Netlify, or other hosting:
- Videos will be included in your repository
- Large videos may slow down your repository
- Consider using a CDN or video hosting service (YouTube, Vimeo) for very large files
- GitHub has a 100MB file size limit (use Git LFS for larger files)

## Alternative: Embed from Video Hosting

If videos are too large, you can host them on:
- **YouTube** (unlisted or public)
- **Vimeo** (free account available)
- **Cloudflare Stream** (paid)
- Then embed using iframe instead of video tag

