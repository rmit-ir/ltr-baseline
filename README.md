
# LTR Baseline

A collection of LTR baselines using various algorithms from publicly availble implementations.

## Results

Tables are orderd by NDCG@10. Statistical significance is indicated using a
pairwise t-test with Bonferroni correction. Entries marked with `*` and `^`
indicate 95% and 99% confidence intervals respectively. Comparisons are
relative to LightGBM.

### Yahoo! Set 1

| Ranker     | Framework | RBP@0.8 | RBP@0.9 | ERR@5   | ERR@10  | ERR@20  | NDCG@5  | NDCG@10 | NDCG@20 |
|------------|-----------|---------|---------|---------|---------|---------|---------|---------|---------|
| GBDT       | XGBoost   | 0.7685^ | 0.6409^ | 0.4600  | 0.4745  | 0.4783  | 0.7439  | 0.7858  | 0.8272  |
| LambdaRank | LightGBM  | 0.7653  | 0.6379  | 0.4616  | 0.4761  | 0.4799  | 0.7425  | 0.7845  | 0.8253  |
| LambdaRank | jforests  | 0.7650  | 0.6377  | 0.4615  | 0.4760  | 0.4798  | 0.7431  | 0.7842  | 0.8256  |
| LambdaMART | QuickRank | 0.7645  | 0.6372  | 0.4603  | 0.4749  | 0.4787  | 0.7408  | 0.7827  | 0.8237  |
| X-DART     | QuickRank | 0.7582^ | 0.6332^ | 0.4546^ | 0.4695^ | 0.4735^ | 0.7237^ | 0.7688^ | 0.8124^ |


### MSLR-WEB10K

| Ranker     | Framework | RBP@0.8 | RBP@0.9 | ERR@5    | ERR@10   | ERR@20   | NDCG@5   | NDCG@10 | NDCG@20 |
|------------|-----------|---------|---------|----------|----------|----------|----------|---------|---------|
| LambdaRank | LightGBM  | 0.6886  | 0.6353  | 0.3548   | 0.3735   | 0.3815   | 0.4724   | 0.4913  | 0.5225  |
| GBDT       | XGBoost   | 0.6917^ | 0.6398^ | 0.3513\* | 0.3702\* | 0.3784\* | 0.4694\* | 0.4893  | 0.5213  |
| LambdaRank | jforests  | 0.6832^ | 0.6306^ | 0.3536   | 0.3724   | 0.3804   | 0.4672^  | 0.4865^ | 0.5180^ |
| LambdaMART | QuickRank | 0.6771^ | 0.6250^ | 0.3470^  | 0.3663^  | 0.3745^  | 0.4582^  | 0.4782^ | 0.5102^ |
| X-DART     | QuickRank | 0.6738^ | 0.6201^ | 0.3458^  | 0.3647^  | 0.3729^  | 0.4552^  | 0.4721^ | 0.5023^ |


### MSLR-WEB30K

| Ranker     | Framework | RBP@0.8 | RBP@0.9 | ERR@5   | ERR@10  | ERR@20  | NDCG@5  | NDCG@10 | NDCG@20 |
|------------|-----------|---------|---------|---------|---------|---------|---------|---------|---------|
| LambdaRank | LightGBM  | 0.6970  | 0.6434  | 0.3698  | 0.3881  | 0.3959  | 0.4865  | 0.5046  | 0.5354  |
| GBDT       | XGBoost   | 0.6989^ | 0.6472^ | 0.3651^ | 0.3836^ | 0.3914^ | 0.4847  | 0.5034  | 0.5349  |
| LambdaRank | jforests  | 0.6938^ | 0.6406^ | 0.3680^ | 0.3864^ | 0.3942^ | 0.4843^ | 0.5025^ | 0.5335^ |
| LambdaMART | QuickRank | 0.6894^ | 0.6358^ | 0.3636^ | 0.3821^ | 0.3899^ | 0.4773^ | 0.4942^ | 0.5243^ |
| X-DART     | QuickRank | 0.6834^ | 0.6294^ | 0.3568^ | 0.3754^ | 0.3834^ | 0.4660^ | 0.4824^ | 0.5125^ |


### Istella-S LETOR

| Ranker     | Framework | RBP@0.8 | RBP@0.9 | ERR@5   | ERR@10  | ERR@20  | NDCG@5  | NDCG@10 | NDCG@20 |
|------------|-----------|---------|---------|---------|---------|---------|---------|---------|---------|
| LambdaRank | LightGBM  | 0.8026  | 0.6213  | 0.7512  | 0.7566  | 0.7572  | 0.7000  | 0.7614  | 0.8215  |
| GBDT       | XGBoost   | 0.8157  | 0.6299  | 0.7311  | 0.7373  | 0.7379  | 0.6798  | 0.7490  | 0.8120  |
