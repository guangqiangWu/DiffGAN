## Multivariate Time Series Anomaly Detection using DiffGAN Model



## Diffusion / DiffGAN

- Train:

> python main.py
>
> ```python
> runnerDiffusion.train()
> runnerDiffGAN.train()
> ```

If you want to resume training from the current checkpoint, you can:

> python main.py --resume_training



- Test:

> python main.py
>
> ```python
> runnerDiffusion.test()
> runnerDiffGAN.test()
> ```

If you want to test a saved model you can:

> python main.py

```python
runnerDiffusion.test('n')  # n-->epoch
runnerDiffGAN.test('n')  # n-->epoch
```



## Run with your own data

- By default, datasets are placed under the "data" folder. If you need to change the dataset, you can modify the dataset path  in file "parser.py". Then you should change the corresponding parameters of models in file "config.yml".

> python main.py  --dataset xx



## Result

- We  use dataset "point_global" for testing demonstration, the runtime environment and model parameters have been configured, you can run "main.py" directly and get the corresponding result.

- For ease of testing, we have placed the pre-trained models in the "saved_models_pre" folder.
