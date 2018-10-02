p = np.array([0.1, 0.0, 0.7, 0.2])
index = np.random.choice([0, 1, 2, 3], p = p.ravel())
This means that you will pick the index according to the distribution:  P(index=0)=0.1,P(index=1)=0.0,P(index=2)=0.7,P(index=3)=0.2

shuffle的另一种方式np.random.shuffle(examples)

可以看下面的莎士比亚诗歌生成