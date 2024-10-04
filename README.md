# HAP Maker

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
```bash

 ██░ ██  ▄▄▄       ██▓███      ███▄ ▄███▓ ▄▄▄       ██ ▄█▀▓█████  ██▀███
▓██░ ██▒▒████▄    ▓██░  ██▒   ▓██▒▀█▀ ██▒▒████▄     ██▄█▒ ▓█   ▀ ▓██ ▒ ██▒
▒██▀▀██░▒██  ▀█▄  ▓██░ ██▓▒   ▓██    ▓██░▒██  ▀█▄  ▓███▄░ ▒███   ▓██ ░▄█ ▒
░▓█ ░██ ░██▄▄▄▄██ ▒██▄█▓▒ ▒   ▒██    ▒██ ░██▄▄▄▄██ ▓██ █▄ ▒▓█  ▄ ▒██▀▀█▄
░▓█▒░██▓ ▓█   ▓██▒▒██▒ ░  ░   ▒██▒   ░██▒ ▓█   ▓██▒▒██▒ █▄░▒████▒░██▓ ▒██▒
 ▒ ░░▒░▒ ▒▒   ▓▒█░▒▓▒░ ░  ░   ░ ▒░   ░  ░ ▒▒   ▓▒█░▒ ▒▒ ▓▒░░ ▒░ ░░ ▒▓ ░▒▓░
 ▒ ░▒░ ░  ▒   ▒▒ ░░▒ ░        ░  ░      ░  ▒   ▒▒ ░░ ░▒ ▒░ ░ ░  ░  ░▒ ░ ▒░
 ░  ░░ ░  ░   ▒   ░░          ░      ░     ░   ▒   ░ ░░ ░    ░     ░░   ░
 ░  ░  ░      ░  ░                   ░         ░  ░░  ░      ░  ░   ░


HAP Video Converter - Simplifying Your Workflow

? Select an option:
❯ Single File
  Batch Files
  Quit
  ```




**HAP Maker** is a specialized video conversion tool designed for **virtual production studios** that frequently utilize HAP videos in their workflows. Whether you're working with high-performance video playback systems such as **Disguise d3**, **Resolume**, or **Unreal Engine**, this tool simplifies the process of converting single or multiple video files into various HAP formats. **HAP Maker** is optimized to provide an efficient solution for studios looking to automate HAP encoding for content pipelines, offering a clear and interactive command-line interface (CLI) that accommodates both single-file and batch processing.

## Key Features

- **Single File and Batch Conversion**: Convert one or multiple video files into HAP, HAP Alpha, or HAP Q formats.
- **User-Friendly CLI**: A simple and interactive command-line interface for easy usage.
- **Progress Tracking**: Real-time progress bar displays percentage completed, estimated time remaining (ETA), and conversion speed.
- **ESC to Cancel**: Abort any ongoing conversion process by pressing the ESC key.
- **Codec Options**: Choose between HAP, HAP Alpha, and HAP Q codecs, with a potential for more formats in future updates.
- **Cross-Platform Support**: Designed to work on Windows, macOS, and Linux environments, given FFmpeg is installed.

## Why HAP Maker?

**HAP Maker** is built with a focus on virtual production environments where high-quality, performance-optimized video formats like HAP are essential. While HAP encoding can be a cumbersome process for artists and technicians, **HAP Maker** simplifies and automates it, enabling fast batch conversions, streamlined workflows, and production-ready assets.

### Roadmap and Future Development

- **New Codec Support**: Plan to add support for other commonly used production codecs like ProRes, CineForm, and more.
- **Automated Workflow Integration**: Provide seamless automation with production pipelines for real-time and non-linear video workflows.
- **Metadata Preservation**: Ensure key metadata such as timecodes, audio tracks, and more are preserved during the conversion process.
- **Enhanced Batch Processing**: Add more flexible options for batch processing large video libraries with custom file naming conventions.
- **GUI Version**: Future versions will include a graphical user interface (GUI) for users who prefer a more visual interaction model.

## Installation

You can install **HAP Maker** by cloning this repository and ensuring you have Python 3.6 or later installed. You'll also need to have **FFmpeg** installed and accessible through your system’s PATH.

1. Clone the repository:
   ```bash
   git clone https://github.com/MGX-Studios/Hap-Maker.git
   cd Hap-Maker
   ```

2. Install the necessary dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure **FFmpeg** is installed and available in your system's PATH. You can download it from [FFmpeg.org](https://ffmpeg.org/download.html).

## Usage

There are two primary ways to use HAP Maker: **interactive CLI mode** or **command-line mode** via flags. Below are the details for both modes:

### 1. Interactive CLI Mode

To launch the interactive CLI, run the following command:

```bash
python hap-maker.py
```

This will display a series of menu options:

- **Single File**: Convert a single video file into a selected HAP codec.
- **Batch Files**: Batch convert multiple video files from a folder.
- **Quit**: Exit the program.

#### Example Flow for Single File Conversion:

1. **Select Input File**: You will be prompted to select the input video file (supported formats include `.mp4`, `.mov`, and `.avi`).
2. **Select Output File**: You will be asked where to save the converted HAP file and its format (HAP, HAP Alpha, or HAP Q).
3. **Monitor Progress**: A progress bar will track the conversion process, displaying the percentage completed, estimated time remaining, and elapsed time.
4. **Completion**: After successful conversion, the message `Complete - Başarıyla tamamlandı!` will appear, signifying a successful HAP conversion.

### 2. Command-Line Mode with Flags

For users who want more control over the conversion process or prefer automation, **HAP Maker** can be run via command-line flags.

#### Command Flags:

- `-i`, `--input`: Specifies the input video file path.
- `-o`, `--output`: Specifies the output file path for the converted video.
- `-c`, `--codec`: Specifies the codec to use for the HAP conversion (`hap`, `hap_alpha`, or `hap_q`).
  
Example usage:
```bash
python hap-maker.py -i /path/to/input/file.mp4 -o /path/to/output/file.mov -c hap
```

This command converts the input file using the **HAP codec** and saves the output at the specified path.

### Progress Bar

During both single file and batch conversions, a **progress bar** is shown in the terminal. The progress bar includes the following features:

- **Percentage**: Displays the current percentage of completion.
- **ETA (Estimated Time of Arrival)**: Shows the estimated remaining time based on the current conversion speed.
- **Elapsed Time**: Tracks the total time spent on the conversion so far.
  
Example:
```
Converting /path/to/video.mp4 (codec: hap) FPS: 50, Duration: 0:01:55, Frame: 5750
|███████████████████████████████████████████████=========================|  73% ETA:  0:00:45
```

### Batch Conversion

**Batch Files** allows you to process an entire folder of video files. Here’s how it works:

1. **Select Input Folder**: Choose the folder containing all video files you want to convert.
2. **Select Output Folder**: Specify where the converted files should be saved.
3. **Choose Codec**: Select one of the HAP codecs (HAP, HAP Alpha, HAP Q).
4. **Batch Processing**: The tool will process each file in the input folder and save the output in the designated folder, with a progress bar showing each file's progress.

### ESC to Cancel

You can press the **ESC** key at any point during the conversion process to abort the conversion. The program will stop immediately, and any ongoing FFmpeg process will be terminated.

## Advanced Features

### 1. Argument-Based Execution

For advanced users or automation, you can pass in arguments directly to convert videos without the interactive CLI. This is useful for integrating **HAP Maker** into larger workflows or scripts. 

```bash
python hap-maker.py --input /path/to/input.mp4 --output /path/to/output.mov --codec hap
```

### 2. Custom Output Naming for Batch Processing

In batch processing, the tool appends the codec type to the output filename to ensure clarity and distinction between files. For example, an input file named `example.mp4` processed with **HAP Q** will output a file named `example_hap_q.mov`.

## Planned Features

Our roadmap includes the following features:

1. **Additional Codec Support**: Support for more codecs such as ProRes and CineForm to meet a wider range of video production needs.
2. **Metadata Preservation**: Ensuring that crucial metadata (e.g., timecode, color space, audio tracks) is retained during conversions.
3. **Automation Integration**: Allow seamless integration with production pipelines for automated conversions.
4. **Enhanced Batch Processing**: Further customization options for batch processing, including automated folder monitoring for real-time conversions.
5. **Graphical User Interface (GUI)**: A planned GUI version to make the tool even more accessible for users preferring a visual interface.

## Contribution

We welcome contributions! If you'd like to contribute to **HAP Maker**, follow these steps:

1. **Fork the repository**.
2. **Clone your fork**:
   ```bash
   git clone https://github.com/yourusername/Hap-Maker.git
   ```
3. **Create a feature branch**:
   ```bash
   git checkout -b new-feature
   ```
4. **Commit your changes** and push them to your fork:
   ```bash
   git commit -m "Add new feature"
   git push origin new-feature
   ```
5. **Open a pull request** and submit your changes for review.

Please ensure your changes are well-documented, and tests are added for any new functionality.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
