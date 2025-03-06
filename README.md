使用说明：
数据预处理：python -m pcdet.datasets.kitti.kitti_dataset create_kitti_infos tools/cfgs/dataset_configs/kitti_dataset.yaml



训练：python train.py --cfg_file ./cfgs/kitti_models/pointpillar.yaml  --batch_size 4 --epochs 50



测试：python test.py --cfg_file cfgs/kitti_models/second.yaml --batch_size 4 --ckpt /home/ubuntu/Fyx/OpenPCDet/output/cfgs/kitti_models/second/default/ckpt/checkpoint_epoch_1.pth

																																																																																																																																		




可视化：python demo.py --cfg_file ./cfgs/kitti_models/second.yaml --ckpt /home/ubuntu/Fyx/OpenPCDet/output/cfgs/kitti_models/second/default/ckpt/checkpoint_epoch_1.pth --data_path /home/ubuntu/Fyx/OpenPCDet/data/kitti/testing/velodyne/000001.bin	
