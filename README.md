paper link: http://alisec-competition.oss-cn-shanghai.aliyuncs.com/competition_papers/20211201/rank10.pdf

![image](https://user-images.githubusercontent.com/49955700/199968902-fd7f61f6-ee0a-43cd-a5f2-9295a11748a5.png)


This work is sponsored by Natural Science Foundation of China(62276242), CAAI-Huawei MindSpore Open Fund(CAAIXSJLJJ-2021-016B), Anhui Province Key Research and Development Program(202104a05020007), and USTC Research Funds of the Double First-Class Initiative(YD2350002001)”。

We use Mindspore to develop our algorithm.


## The generated partial image candidate set

![image](https://user-images.githubusercontent.com/49955700/200109515-b8193a0c-d1b6-494f-9a57-114d6f594ffa.png)

## Experiment results
![image](https://user-images.githubusercontent.com/49955700/200109532-ccae6371-8a6b-450f-9c07-29868043b9ed.png)


## How to run

1. Obtain all Cifar10 data from the official website to the folder CIFAR-10-FANs-PY;
2. Create two empty folders.  new_data and train_model;
3. Run gen_corr_data.ipynb to generate corruption data;
4. Run final_gen_data_iter to generate the first generation of the data;
5. Run train.py to generate the first generation model;
6. Generate the next generation of the data.
7. Loop 5 ~ 6 until num = 6. In general, it takes 5 times to train the model to get the final submitted model, and 4 times to get the final submitted data.npy.
