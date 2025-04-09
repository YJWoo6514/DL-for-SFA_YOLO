* Train
python train.py --cache --batch 32 --cfg models/yolov5s.yaml --name yolov5s_512_exp --weights yolov5s.pt --epochs 100

python val.py --weights best/yolov5s.pt --name yolov5s_512_exp

python detect.py --weights runs/train/yolov5m_512_exp4/weights/best.pt --name yolov5m_512_exp --img 512