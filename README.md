# Behavior Based Consumption Profiles (BBCP)

Despite the increase in the efficiency of energy consumption in information and communication technology, software execution
and its constraints are responsible for how energy is consumed in hardware hosts. Consequently, researchers have promoted the
development of sustainable software with new development methods and tools to lessen its hardware demands. However, the
approaches developed so far lack cohesiveness along the stages of the Software Development Life Cycle (SDLC) and exist outside
of a holistic method for Green Software Development (GSD). In addition, there is a severe lack of approaches that target the
analysis and design stages of the SDLC, leaving software architects and designers unsupported. We introduce here our
Behavior-Based Consumption Profiles (BBCP) external Domain-Specific Language (DSL), aimed at assisting software architects
and designers in modeling the behavior of software. The models generated with our external DSL contain multiple sets of properties
that characterize features of the software’s behavior. In contrast to other modeling languages, our BBCP emphasizes how time and
probability are involved in software execution and its evolution over time, helping its users to gather an expectation of software
usage and hardware consumption from the initial stages of software development. 

# Sample models created with Insight Maker

## Game Stream Profile
To provide an example that demonstrates a realistic use case for our BBCP, we analyzed an existing application from the perspective of service-oriented architectures (SOA) and created a couple of example BBCPs to simulate the behavior of the target application Geforce Now, a cloud gaming service developed by NVIDIA. In cloud gaming, the hardware responsible for running the game and managing inputs and outputs from and to the consumer is in the cloud (a computer cluster in the network), making use of software as a service delivery model (SaaS) based on subscriptions. 

The user provides hardware peripheral input such as mouse movement and keyboard strokes to the cloud through the internet, which in turn gets processed to provide the user with an output, usually in the form of video and audio, also sent over the internet. We chose this application due to the popularity of streaming platforms and its easy architectural abstraction into components. From a SOA perspective, there are 2 services that we profiled: the catalog service and the stream service. 

The catalog service is responsible for offering the user a catalog of the available games to play. Once a game is selected, the game stream service is responsible for the rest of the I/O operations until the user decides to stop playing. The objective of the example is to obtain an estimation of the energy consumption of the game stream service using BBCPs in coalition with the time constraints that the subscription service employs to limit the behavior of the user. 
- Game Stream Profile (1st Cycle): https://insightmaker.com/insight/3RUGFBRxFbB1xt7szTrIGY/Game-stream-service
- Game Stream Profile (2nd Cycle):  https://insightmaker.com/insight/2LwDgPTxw8HjluWrhBeiDn/Game-stream-service-second-cycle
- Catalog Service (Shell - 1st Cycle): https://insightmaker.com/insight/3ezUM7LGPJPwK4kw7hRQ2p/Catalog-Service-Shell
- Catalog Service (Shell - 2nd Cycle): https://insightmaker.com/insight/2vKeUIARREkXPnJF5PWBd7/Catalog-service-shell-second-cycle
> Disclamer: Some of the models could stop working due to the changes made by the developers of Insight Maker.
