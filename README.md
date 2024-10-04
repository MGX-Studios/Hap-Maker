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

HAP Video Converter - Simplifying Your Workflow 🚀

🎬 **Select an option**:
❯ 🎥 Single File
  🎞️ Batch Files
  ❌ Quit
```

---

**🎥 HAP Maker** is a specialized video conversion tool designed for **virtual production studios** that frequently utilize HAP videos in their workflows. Whether you're working with high-performance video playback systems such as **Disguise d3**, **Resolume**, or **Unreal Engine**, this tool simplifies the process of converting single or multiple video files into various HAP formats. **HAP Maker** is optimized to provide an efficient solution for studios looking to automate HAP encoding for content pipelines, offering a clear and interactive command-line interface (CLI) that accommodates both single-file and batch processing.

## ✨ Key Features

- 🔄 **Single File and Batch Conversion**: Convert one or multiple video files into HAP, HAP Alpha, or HAP Q formats.
- 🖥️ **User-Friendly CLI**: A simple and interactive command-line interface for easy usage.
- ⏱️ **Progress Tracking**: Real-time progress bar displays percentage completed, estimated time remaining (ETA), and conversion speed.
- ⛔ **ESC to Cancel**: Abort any ongoing conversion process by pressing the ESC key.
- 🎥 **Codec Options**: Choose between HAP, HAP Alpha, and HAP Q codecs, with a potential for more formats in future updates.
- 🖥️ **Cross-Platform Support**: Works on Windows, macOS, and Linux environments (with FFmpeg installed).

## 🚀 Why HAP Maker?

**HAP Maker** is built with a focus on virtual production environments where high-quality, performance-optimized video formats like **HAP** are essential. While HAP encoding can be a cumbersome process for artists and technicians, **HAP Maker** simplifies and automates it, enabling fast batch conversions, streamlined workflows, and production-ready assets.

---

### 📅 Roadmap & Future Development

- 🆕 **New Codec Support**: Plan to add support for production codecs like **ProRes**, **CineForm**, and more.
- 🤖 **Automated Workflow Integration**: Seamless automation with production pipelines for real-time and non-linear video workflows.
- 🎞️ **Metadata Preservation**: Ensure that key metadata such as timecodes, audio tracks, and more are preserved.
- 📂 **Enhanced Batch Processing**: Add flexible options for large video libraries with custom file naming conventions.
- 🖼️ **GUI Version**: Future versions will include a graphical user interface (GUI) for users preferring a more visual interaction model.

---

## 📦 Installation

You can install **HAP Maker** by cloning this repository and ensuring you have **Python 3.6** or later installed. You’ll also need **FFmpeg** installed and accessible through your system’s PATH.

1. **Clone the repository**:
   ```bash
   git clone https://github.com/MGX-Studios/Hap-Maker.git
   cd Hap-Maker
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Ensure FFmpeg is installed**:  
   Download it from [FFmpeg.org](https://ffmpeg.org/download.html) and ensure it’s in your system’s PATH.

---

## 🎛️ Usage

There are two primary ways to use **HAP Maker**: **interactive CLI mode** or **command-line mode** via flags.

### 1. **Interactive CLI Mode** 🎮

To launch the interactive CLI, run:
```bash
python hap-maker.py
```

This will display a menu with the following options:

- 🎥 **Single File**: Convert a single video file into a selected HAP codec.
- 🎞️ **Batch Files**: Batch convert multiple video files from a folder.
- ❌ **Quit**: Exit the program.

#### Example Flow for Single File Conversion:

1. **Select Input File**: You will be prompted to select the input video file (formats: `.mp4`, `.mov`, `.avi`).
2. **Select Output File**: Specify where to save the converted HAP file and its format (**HAP**, **HAP Alpha**, or **HAP Q**).
3. **Monitor Progress**: Watch the progress bar for conversion status.
4. 🎉 **Completion**: After successful conversion, the message `Complete - Başarıyla tamamlandı!` will appear, confirming success.

---

### 2. **Command-Line Mode with Flags** 🛠️

For users who want more control or prefer automation, **HAP Maker** can be run via command-line flags.

#### Command Flags:

- `-i`, `--input`: Specifies the input video file path.
- `-o`, `--output`: Specifies the output file path.
- `-c`, `--codec`: Specifies the codec (`hap`, `hap_alpha`, or `hap_q`).

Example usage:
```bash
python hap-maker.py -i /path/to/input/file.mp4 -o /path/to/output/file.mov -c hap
```

---

### ⏳ **Progress Bar** 🏁

During both single and batch conversions, a **progress bar** is shown in the terminal. It includes:

- ✅ **Completion Percentage**
- ⏲️ **ETA (Estimated Time of Arrival)**
- ⏳ **Elapsed Time**

Example:
```
Converting /path/to/video.mp4 (codec: hap) FPS: 50, Duration: 0:01:55, Frame: 5750
|██████████████████████████████████████| 73% ETA:  0:00:45
```

---

### 📁 **Batch Conversion**

With **Batch Files**, you can process an entire folder of videos:

1. **Select Input Folder**: Choose the folder with video files.
2. **Select Output Folder**: Specify where to save the converted files.
3. **Choose Codec**: Select the HAP codec (**HAP**, **HAP Alpha**, **HAP Q**).
4. **Batch Processing**: The tool will convert each file in the folder and save it, with a progress bar for each file.

### ⛔ **ESC to Cancel**

You can press **ESC** at any point during the conversion to abort. The program will stop immediately, terminating any ongoing FFmpeg process.

---

## ⚙️ **Advanced Features**

### 1. **Argument-Based Execution** 🚀
For advanced users or automation, you can pass arguments directly:
```bash
python hap-maker.py --input /path/to/input.mp4 --output /path/to/output.mov --codec hap
```

### 2. **Custom Output Naming for Batch Processing** 📝

During batch processing, the codec type is appended to the output filename for clarity. For example, `example.mp4` processed with **HAP Q** will output as `example_hap_q.mov`.

---

## 🎯 **Planned Features**

1. **Additional Codec Support**: Support for **ProRes**, **CineForm**,

 and more.
2. **Metadata Preservation**: Retain key metadata such as timecodes, color spaces, and audio tracks.
3. **Automation Integration**: Seamless integration with production pipelines.
4. **Enhanced Batch Processing**: More options, including folder monitoring.
5. **Graphical User Interface (GUI)**: A planned GUI version for visual interaction.

---

## 🤝 **Contribution**

We welcome contributions! Follow these steps to contribute to **HAP Maker**:

1. **Fork the repository**.
2. **Clone your fork**:
   ```bash
   git clone https://github.com/yourusername/Hap-Maker.git
   ```
3. **Create a feature branch**:
   ```bash
   git checkout -b new-feature
   ```
4. **Commit your changes** and push to your fork:
   ```bash
   git commit -m "Add new feature"
   git push origin new-feature
   ```
5. **Open a pull request** and submit your changes for review.

---

## 📝 **License**

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.
