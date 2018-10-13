# CarND Capstone Test frozen model

## Generated using pythonv2, Tensorflow 1.10

### Caveats
This model has been trained on very few steps, Do NOT expect this model to recognize traffic lights
Goal of this model is to test whether model generated from Python27 can work with ROS Udacity simulator

#### Model training command
python object_detection/legacy/train.py --pipeline_config_path=config/faster_rcnn_inception_v2_sim.config --train_dir=data/sim_training_data/sim_data_capture

### Model generation command
python object_detection/export_inference_graph.py --pipeline_config_path=config/faster_rcnn_inception_v2_sim.config --trained_checkpoint_prefix=data/sim_training_data/sim_data_capture/model.ckpt-49 --output_directory=frozen_sim_pythonv27

