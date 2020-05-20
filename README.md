# README

How to use Vilbert with a single image and single question architecture.

Download and unzip the following archive (it includes the detectron needed for the mask-rcnn network):
  https://drive.google.com/open?id=1svdJo1dP2qGZ8MfD2fIepn5NCp_jlX6U

Install the prerequisites from requirements.txt.

Follow the README.MD from inside the archive.

To infer with only a image and a question:

python eval_tasks.py --bert_model bert-base-uncased --from_pretrained ./multi_task_model.bin --output_dir ./output/ --config_file ./config/bert_base_6layer_6conect.json --num_workers 1 --tasks 1 --batch_size 1 --split val --image_path <path_to_img> --question <question as a string>

