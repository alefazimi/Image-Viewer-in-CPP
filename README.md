# Image Viewer in C++

\documentclass{article}
\usepackage[utf-8]{inputenc}

\title{ProImageViewer}
\author{}
\date{}

\begin{document}

\maketitle

\section*{Overview}

\textbf{ProImageViewer} is a professional-grade desktop image viewer built with \textbf{C++}, \textbf{Qt6}, and \textbf{OpenCV}. It provides an intuitive interface for browsing, editing, and managing images with advanced image processing capabilities.

\section*{Features}

\begin{itemize}
    \item \textbf{Image Navigation}: Browse images in directories with next/previous navigation
    \item \textbf{Zoom \& Pan}: Zoom in/out and fit-to-window display modes
    \item \textbf{Image Editing}:
    \begin{itemize}
        \item Brightness \& Contrast adjustment with live sliders
        \item Saturation control
        \item Blur effects
        \item Grayscale toggle
        \item Sharpen filter
        \item 90\textdegree{} rotation
    \end{itemize}
    \item \textbf{Crop Tool}: Interactive crop mode with rubber band selection
    \item \textbf{Undo/Redo System}: Full edit history with unlimited undo/redo
    \item \textbf{File Operations}: Open, save, and save-as functionality
    \item \textbf{Settings Persistence}: Automatically saves window state and user preferences
    \item \textbf{Directory Scanner}: Automatic detection of all supported image formats in directories
\end{itemize}

\section*{Supported Image Formats}

JPEG, PNG, BMP, TIFF, GIF, and other OpenCV-supported formats

\section*{Project Structure}

\begin{verbatim}
├── CMakeLists.txt          # Build configuration
├── main.cpp                # Application entry point
├── MainWindow.h/cpp        # Main UI window with editing features
├── DirectoryScanner.h/cpp  # Directory browsing utility
├── ImageUtils.h            # Image processing utilities
└── build/                  # Build artifacts
\end{verbatim}

\section*{Requirements}

\begin{itemize}
    \item \textbf{C++17} or later
    \item \textbf{Qt6} (Widgets, Concurrent modules)
    \item \textbf{OpenCV} 4.0+
    \item \textbf{CMake} 3.16+
\end{itemize}

\section*{How to Build \& Run}

\begin{verbatim}
# Navigate to the project directory
cd ImageViewer

# Create build directory
mkdir -p build
cd build

# Configure and build
cmake ..
make

# Run the application
./ProImageViewer
\end{verbatim}

\section*{Usage}

\begin{enumerate}
    \item \textbf{Open Image}: File \textrightarrow{} Open or drag-and-drop
    \item \textbf{Browse Directory}: Navigate through images using next/previous buttons
    \item \textbf{Edit}: Use sliders and tools to adjust brightness, contrast, saturation, blur
    \item \textbf{Rotate}: Click the rotate button for 90\textdegree{} clockwise rotation
    \item \textbf{Crop}: Toggle crop mode, select area with mouse, press crop
    \item \textbf{Undo/Redo}: Revert or redo any edits
    \item \textbf{Save}: Save edited images back to disk
\end{enumerate}

\end{document}
