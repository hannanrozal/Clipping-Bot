# AI Clip Splitter

A powerful tool for automatically generating engaging video clips using AI. This tool uses OpenAI's GPT models to analyze video content and suggest the most engaging moments to clip, along with Whisper for accurate transcription.

## Features

### Video Downloader
- Download videos from YouTube and other platforms
- Select video quality and format
- Download playlists
- Extract audio only
- Progress tracking
- Custom output directory

### Clip Splitter
- AI-powered clip generation
- Transcript caching
- Smart model filtering
- GPU acceleration
- Custom clip count range
- Progress tracking
- Excel output with clip suggestions

### Metadata Generator (New!)
- Process multiple videos in a directory
- Automatic transcription using Whisper
- AI-generated metadata for each video:
  - Engaging titles
  - Detailed descriptions
  - Relevant keywords
  - Content summaries
- Excel output with all metadata
- Transcript caching for faster processing
- GPU acceleration support

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ai-clip-splitter.git
cd ai-clip-splitter
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Set up your OpenAI API key:
   - Create a `.env` file in the project directory
   - Add your OpenAI API key: `OPENAI_API_KEY=your_api_key_here`
   - Or set it in the application's Settings menu

## Usage

### Video Downloader
1. Click on the "Video Downloader" tab
2. Enter the video URL
3. Click "Fetch Info" to get video details
4. Select download options (quality, format, etc.)
5. Choose output directory
6. Click "Download"

### Clip Splitter
1. Click on the "Clip Splitter" tab
2. Select a video file
3. Choose output directory
4. Select GPT model
5. Set minimum and maximum clip counts
6. Click "Process Video"
7. Wait for processing to complete
8. Find generated clips in the output directory

### Metadata Generator
1. Click on the "Metadata Generator" tab
2. Select input directory containing videos
3. Choose output directory for metadata file
4. Select GPT model
5. Click "Generate Metadata"
6. Wait for processing to complete
7. Find metadata in the generated Excel file

## Settings

Access settings through the menu bar:
- API Settings: Configure OpenAI API key
- GPU Settings: Enable/disable GPU acceleration
- Processing Settings: Configure Whisper model and encoding options
- Output Settings: Set default output directories

## Requirements

- Python 3.8 or higher
- OpenAI API key
- FFmpeg (for video processing)
- GPU with CUDA support (optional, for faster processing)

## Dependencies

- pandas
- moviepy
- openai-whisper
- openai
- openpyxl
- python-dotenv
- PyQt6
- yt-dlp

## Notes

- The application uses GPU acceleration when available for faster processing
- Transcripts are cached to avoid re-processing the same videos
- The clip splitter uses AI to identify the most engaging moments
- The metadata generator creates SEO-friendly content for your videos

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 🙏 Acknowledgments

- OpenAI for GPT and Whisper models
- PyQt6 for the GUI framework
- MoviePy for video processing
- All other open-source libraries used in this project 
