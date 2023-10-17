# Jetpack4.6_ONNXRuntime_TensorRT_Installation
Jetpack 4.6 ONNX Runtime TensorRT Installation 
 
Jetpack 4.6  
CUDA 10.2  
ONNXRuntime 1.6.0  
TensorRT 7.1.3  


dpkg -i libs/{\*}  
git clone https://github.com/microsoft/onnxruntime.git  
git checkout v.1.6.0  
git submodule update --init --recursive  
./build.sh  --build_shared_lib --config Release --update --build --parallel --use_tensorrt --tensorrt_home /usr/lib/aarch64-linux-gnu --cuda_home /usr/local/cuda --cudnn_home /usr/lib/aarch64-linux-gnu  
