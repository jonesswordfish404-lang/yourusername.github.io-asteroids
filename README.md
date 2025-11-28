# CFF Compression Tool

A powerful file compression and archiving tool with advanced features including FFmpeg media optimization, ISO support, and password protection.

## Features

### Core Compression
- **CFF Format**: Custom Compressed File Format with high compression ratios
- **Password Protection**: AES-256 encryption for secure file storage
- **Large File Support**: Handle files over 2GB with ZIP64 format
- **Folder Structure**: Preserves original directory structure
- **Progress Tracking**: Real-time compression progress with file size display

### Media Optimization
- **FFmpeg Integration**: Automatic video optimization for 40-60% better compression
- **H.265 Encoding**: Modern HEVC codec for maximum compression
- **Smart Detection**: Automatically identifies media files (MP4, AVI, MKV, MOV, etc.)
- **Quality Preservation**: Maintains visual quality while reducing file size

### ISO Tools
- **ISO Extraction**: Extract files from ISO images (ISO9660 and UDF formats)
- **CFF to ISO Conversion**: Convert compressed archives to ISO format
- **Windows ISO Support**: Full support for Windows 10/11 installation ISOs
- **Bootable ISO**: Maintains bootable properties when converting

### User Interface
- **Modern Design**: Clean, intuitive tabbed interface
- **Password Visibility Toggle**: Eye buttons to show/hide passwords
- **Drag & Drop Support**: Easy file selection
- **Real-time Status Updates**: Always know what's happening
- **Responsive UI**: Never freezes - smooth operation throughout

## Requirements

- **Operating System**: Windows 7 or later
- **.NET Framework**: 4.7.2 or higher
- **FFmpeg**: Optional - for media optimization (place ffmpeg.exe in app folder)

## Installation

1. Download the latest release
2. Extract to your preferred location
3. (Optional) Place `ffmpeg.exe` in the same folder for media optimization
4. Run `CFFCompression.exe`

## Usage

### Compressing Files

1. Go to the **Compress** tab
2. Click **Add Files** to select files to compress
3. Choose output location with **Browse**
4. (Optional) Enter a password for encryption
5. (Optional) Enable FFmpeg optimization for media files
6. Click **Compress Files**

### Extracting Files

1. Go to the **Extract** tab
2. Click **Browse** to select a CFF file
3. Click **Extract Files** and choose output folder
4. (Optional) Enter password if file is encrypted

### ISO Tools

**Extract ISO:**
1. Go to the **ISO Tools** tab
2. Select an ISO file
3. Click **Extract ISO** and choose output folder

**Convert CFF to ISO:**
1. Select a CFF file
2. Choose output location
3. Click **Convert CFF to ISO**

## Technical Details

- **Compression**: DEFLATE algorithm with optimal compression level
- **Encryption**: AES-256 with PBKDF2 key derivation
- **ISO Formats**: ISO9660 and UDF support via DiscUtils
- **Video Encoding**: H.265/HEVC via FFmpeg
- **File Format**: Custom CFF format with version 2 support for large files

## Performance

- **Speed**: 20-50 MB/s compression (single-threaded)
- **Media Optimization**: 40-60% additional space savings for videos
- **Large Files**: No size limits for unencrypted files
- **Encrypted Files**: Up to 2GB (memory limitation)

## Third-Party Software

This software uses the following open-source libraries:

- **DiscUtils** - Copyright (c) Kenneth Bell and contributors  
  Licensed under the MIT License  
  For ISO file system operations

- **FFmpeg** - Copyright (c) FFmpeg developers  
  Licensed under LGPL 2.1+  
  For video optimization  
  https://ffmpeg.org/legal.html

## Known Limitations

- Encrypted files over 2GB must be loaded into memory (not recommended)
- FFmpeg must be provided separately (licensing requirement)
- Single-threaded compression (reliable but not fastest)

## Future Enhancements

- Multi-threaded compression
- Cloud backup integration
- Automatic backup scheduling
- File deduplication
- Archive browsing without extraction

## License

This project is licensed under the MIT License - see the [LICENSE.txt](LICENSE.txt) file for details.

## Author

[Your Name/Company Name]

## Support

For issues, questions, or suggestions:
- Open an issue on GitHub
- Email: [your-email@example.com]

## Version History

### Version 1.0 (2025)
- Initial release
- Core compression and extraction
- FFmpeg media optimization
- ISO tools (extract and convert)
- Password protection
- Modern UI with eye buttons
- UDF ISO support for Windows ISOs

---

**Built with ❤️ using Visual Basic .NET**
