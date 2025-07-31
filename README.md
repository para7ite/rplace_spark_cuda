<div align="center">
<h1 align="center">🚀 r/place Timelapse with PySpark & NVIDIA RAPIDS 🚀</h1>
<p align="center">
Recreating the entire 2023 r/place canvas from 132 million pixels, accelerated by the power of GPUs.
</p>
</div>

<p align="center">
<img alt="License" src="https://img.shields.io/badge/License-MIT-yellow.svg"/>
<img alt="Python" src="https://img.shields.io/badge/Python-3.10-blue.svg"/>
<img alt="Framework" src="https://img.shields.io/badge/Framework-PySpark-orange"/>
<img alt="GPU Acceleration" src="https://img.shields.io/badge/GPU%20Acceleration-NVIDIA%20RAPIDS-brightgreen"/>
<img alt="Platform" src="https://img.shields.io/badge/Platform-Linux-lightgrey"/>
</p>
✨ Features

    Blazing Fast GPU Acceleration: Leverages the NVIDIA RAPIDS Accelerator for PySpark to crush data processing tasks on the GPU.

    Massive Data Crunching: Effortlessly processes the entire r/place dataset of over 132 million pixel updates.

    Stunning Timelapse Generation: Produces a high-quality, dynamic video of the canvas's evolution from the first pixel to the last.

    Scalable by Design: Built on Apache Spark, ready to scale from a single workstation to a full-blown cluster.

🚀 Performance

Processing 132 million records is no small feat. Traditional CPU-based processing can be a bottleneck. This is where NVIDIA RAPIDS comes in.

    By offloading heavy-duty operations like filtering, sorting, and aggregations to the GPU, we achieve a massive performance boost. This makes it feasible to analyze the entire dataset and render the final video in a fraction of the time it would take on a CPU.

🛠️ Getting Started

Follow these steps to get the project running on your local machine.
📦 Prerequisites

    Anaconda or Miniconda: The recommended package manager.

    Apache Spark: The core distributed computing engine.

    NVIDIA GPU: A CUDA-enabled NVIDIA GPU is required.

    NVIDIA RAPIDS: The magic behind the GPU acceleration.

        ⚠️ Important Note: RAPIDS is officially supported on Linux only.

    Jupyter: For an interactive experience with the notebook.

⚙️ Installation

    Clone the Fortress: Get the code on your local machine.

    git clone https://github.com/para7ite/rplace_spark_cuda.git
    cd rplace_spark_cuda

    Set Up Your Environment: Create a dedicated conda environment.

    conda create -n rapids-24.12 python=3.10
    conda activate rapids-24.12

    Install the Power (RAPIDS):

    # This command installs RAPIDS and its dependencies
    conda install -c rapidsai -c conda-forge -c nvidia rapids=24.12 python=3.10 cudatoolkit=11.8

    Install Other Tools:

    pip install pyspark matplotlib cupy

▶️ Usage

    Launch Jupyter:

    jupyter notebook

    Open rplace_gpu.ipynb and run the cells from top to bottom.

    Witness the Creation: The script will download the data, process it, and save the final timelapse as animated_canvas.mp4 in the project directory.

🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.
📄 License

This project is licensed under the MIT License. See the LICENSE file for details.
🎬 Video Output

<video src="https://github.com/para7ite/rplace_spark_cuda/raw/main/animated_canvas.mp4" controls="controls" style="max-width: 720px;">Here's the final result. The full animated_canvas.mp4 will be generated when you run the notebook.
</video>
