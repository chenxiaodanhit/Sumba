
## Get Started

1. Install Pytorch and necessary dependencies.
```
pip install -r requirements.txt
```
2. Train the model.
   
 ``` 
python -u run_Sumba.py  --is_training 1 --root_path ./dataset/electricity/  --data_path electricity.csv --model_id ECL_168_3_Sumba --model Sumba --data custom --features M   --seq_len 168  --label_len 84 --pred_len 3 --num_nodes 321 --subgraph_size 20 --des 'Exp'  --batch_size 8 --learning_rate 0.0005 --itr 1
``` 

3. Test the model.
   
 ``` 
python -u run_Sumba.py  --is_training 0 --root_path ./dataset/electricity/  --data_path electricity.csv --model_id ECL_168_3_Sumba --model Sumba --data custom --features M   --seq_len 168  --label_len 84 --pred_len 3 --num_nodes 321 --subgraph_size 20 --des 'Exp'  --batch_size 8 --learning_rate 0.0005 --itr 1
``` 
