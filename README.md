# webgpu-pipeline-electron

The example is ported from tfjs-examples/gpu-pipeline https://github.com/tensorflow/tfjs-examples/tree/master/gpu-pipeline, and could run on electron app based on tfjs webgpu backend.
This demo shows a high performance webgpu pipeline with TF.js. In this example, the pipeline takes a camera stream as input, then feeds to a <a href="https://github.com/tensorflow/tfjs-models/tree/master/body-segmentation">segmentation model</a> from tfjs-models. The output of the model is then fed to a mask processing step to mask the background with purple. And then the result is painted on the canvas.
For details on how to keep the tensor data on GPU, see our [optimization doc](https://github.com/tensorflow/tfjs/blob/master/docs/OPTIMIZATION_PURE_GPU_PIPELINE.md).
