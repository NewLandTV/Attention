# Attention

Implementing Attention Is All You Need with PyTorch.

## Train

```sh
python Train.py  --n=6 --d_model=512 --d_ff=8 --h=8 --d_k=64 --d_v=64 --p_drop=0.1 \
                 --e_ls=0.1 --epoch=1 --batch_size=128 --warmup_steps=4000 \
                 --root_data_path=".Data" --model_path="./Model.pb" --use_small_data
```

## Test

```sh
python Test.py --model_path="./Model.pb" --root_data_path=".Data" --use_small_data --max_seq_len=5000
```