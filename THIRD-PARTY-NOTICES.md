# Third-party software in PariPariVault

PariPariVault itself is free to use but not open source (see `LICENSE`). The Windows build bundles the components below,
each under its own license. Their source code is available from the linked projects.

| Component | License | Project |
|---|---|---|
| Python 3.12 runtime | PSF License | https://www.python.org |
| yt-dlp | Unlicense | https://github.com/yt-dlp/yt-dlp |
| FFmpeg (LGPL build by BtbN, unmodified, shared DLLs) | LGPL 2.1 or later | https://ffmpeg.org · build: https://github.com/BtbN/FFmpeg-Builds |
| OpenH264 (inside the FFmpeg build) | BSD 2-Clause | https://github.com/cisco/openh264 |
| FastAPI / Starlette | MIT / BSD 3-Clause | https://github.com/fastapi/fastapi |
| Uvicorn | BSD 3-Clause | https://github.com/encode/uvicorn |
| Pydantic | MIT | https://github.com/pydantic/pydantic |
| pywebview | BSD 3-Clause | https://github.com/r0x0r/pywebview |
| pythonnet / clr-loader | MIT | https://github.com/pythonnet/pythonnet |
| pystray | LGPL 3.0 | https://github.com/moses-palmer/pystray |
| Pillow | MIT-CMU | https://github.com/python-pillow/Pillow |
| faster-whisper | MIT | https://github.com/SYSTRAN/faster-whisper |
| CTranslate2 | MIT | https://github.com/OpenNMT/CTranslate2 |
| Silero VAD model (in faster-whisper) | MIT | https://github.com/snakers4/silero-vad |
| PyAV (with its FFmpeg libraries) | BSD 3-Clause / LGPL | https://github.com/PyAV-Org/PyAV |
| ONNX Runtime | MIT | https://github.com/microsoft/onnxruntime |
| RapidOCR | Apache 2.0 | https://github.com/RapidAI/RapidOCR |
| PaddleOCR models (PP-OCR) | Apache 2.0 | https://github.com/PaddlePaddle/PaddleOCR |
| NumPy | BSD 3-Clause | https://numpy.org |
| curl_cffi | MIT | https://github.com/lexiforest/curl_cffi |

The LGPL components (FFmpeg, pystray) are shipped as separate, replaceable files: FFmpeg as DLLs in
`_internal/tools/ffmpeg`, pystray as Python modules. You may replace them with your own builds.

## Downloaded on request, not bundled

When you turn on speech search, PariPariVault downloads these from their official sources:

| Component | License | Source |
|---|---|---|
| Whisper models (large-v3-turbo, small) converted for CTranslate2 | MIT | https://huggingface.co/mobiuslabsgmbh/faster-whisper-large-v3-turbo · https://huggingface.co/Systran/faster-whisper-small |
| NVIDIA CUDA runtime, cuBLAS, cuDNN, NVRTC, nvJitLink (only with an NVIDIA GPU) | NVIDIA license agreements (shown on PyPI) | https://pypi.org/project/nvidia-cublas-cu12/ and related packages |

Newer yt-dlp versions are downloaded from https://pypi.org/project/yt-dlp/ (Unlicense).

PariPariVault is not affiliated with, endorsed by or connected to TikTok or ByteDance.
