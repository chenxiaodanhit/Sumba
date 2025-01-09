# Sumba (NeurIPS 2024)
The code for paper: [Structured Matrix Basis for Multivariate Time Series Forecasting with Interpretable Dynamics](https://openreview.net/pdf?id=co7DsOwcop). 

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

# Citation

```
@inproceedings{Sumba, 
   title={Structured Matrix Basis for Multivariate Time Series Forecasting with Interpretable Dynamics},
  author={Chen, Xiaodan and Li, Xiucheng and Chen, Xinyang and Li, Zhijun},
  booktitle={The Thirty-eighth Annual Conference on Neural Information Processing Systems},
  year={2024}
}
```
