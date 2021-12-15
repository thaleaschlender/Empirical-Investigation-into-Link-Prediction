# Empirical-Investigation-into-Link-Prediction

Networks can capture and describe many real world domains from traffic over social networks to molecular networks. Hence, a substantial amount of research has gone into investigating how to utilise these networks. One key aspect to consider is how networks evolve over time. This paper investigates the problem of link prediction, which tries to predict whether two unconnected nodes become connected in the future. Specifically, this problem addresses: given two pre-existing yet unconnected nodes at a certain point in time, what is their likelihood to be connected in the future? This has many potential applications from marketing in social media to drug activity analysis [2]. As such, Hasan et al [1] propose a supervised feature based non-linear classification method. This paper builds on their work by providing an empirical investigation into their method, which was overlooked by the original work. Using 3 covert datasets, this paper investigates the performances of 4 link prediction baselines using different perspectives (including the recent state-of-the-art Node2Vec [3]). 

Further, a key challenge in link prediction is the imbalance between positive and negative link examples. Imbalanced classes can cause features of the minority class to not be learned efficiently, in addition to causing misleading evaluation metric scores. As such, three sampling approaches are investigated. 

We find that Hasan et al's method outperforms all other baselines on balanced samples. Moreover, we examine the impact of different imbalances on their method. Lastly, we call for more research in sampling approaches.

Note that the jupyter notebooks denote which datasets corresponds to which project (PIRA, Conflict, Escort).

Please find the Feature visualisations in the conlfict notebook.

References
[1] Al Hasan, M., Chaoji, V., Salem, S., & Zaki, M. (2006, April). Link prediction using supervised learning. In SDM06: workshop on link analysis, counter-terrorism and security (Vol. 30, pp. 798-805).
[2] Liben‐Nowell, D., & Kleinberg, J. (2007). The link‐prediction problem for social networks. Journal of the American society for information science and technology, 58(7), 1019-1031.
[3] Grover, A., & Leskovec, J. (2016, August). node2vec: Scalable feature learning for networks. In Proceedings of the 22nd ACM SIGKDD international conference on Knowledge discovery and data mining (pp. 855-864).
