# Problem Formulation

The foundation of designing a fair and effective incentive mechanism lies in formulating the incentive problem using appropriate theoretical frameworks such as game theory models, auction models, or other relevant models.

One prominent theoretical framework utilized in Federated Learning is the Stackelberg game. In Federated Learning with Stackelberg game, the task requester assumes the role of the leader, while the clients act as followers. Here, the leader announces a strategy aimed at maximizing model performance, while clients base their actions on the leader's strategy, focusing on maximizing their resource utility to receive rewards.

Another approach, Federated Learning using auction theory, treats the task requester as an auctioneer and the clients as bidders. In this setup, the task requester initiates a task, and clients submit bids along with their computing costs and available resources. The task requester then determines the winner, assigns the task, and rewards the selected client. Some approaches uses auction theory to help aggregators calculate the optimal set of clients to maximize model performance within a limited budget.

In addition to game theory and auction theory, alternative approaches exist for formulating incentive mechanisms. For instance, incentive mechanism can be formulated as a social welfare maximization problem. Furthermore, survey studies highlight additional theoretical frameworks such as contest theory and contract theory.
