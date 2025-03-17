# Statistical modelling
Examples of creating statistical models in R to develop predictive models for analysis. Most of these models are taken from a research project which analysed the effect of the presence/absence of a gut microbiome on exercise (flight) in bees. The probabilty of initiating flight was also analysed. The variables that were taken into considertion for the models included sex, colony (multiple colonies were used ), bee size, amount of sucrose consumed prior to flight, and the presence or absence of a gut.



<br />
<h2>Linear modelling</h2>


<p align="center">
GLM (Generalised Linear Model) in R 
<br/>
<img src="https://imgur.com/NFM1W4W.png" height="80%" width="80%" />
<br />
Model call: glmer(Distance..m. ~ Sex + Mean.Speed + (1|Intertegular.distance..mm.) + (1|Mill) + (1|Colony), nAGQ = 0, family = Gamma(link = log), data = GF_d_F)
<br />
<br />


<h2>Binomial modelling</h2>

<p align="center">
Binomial Model - Example 1
<br/>
<img src="https://imgur.com/q0l9f9O.png" height="80%" width="80%" />
<br />
Model call: sucro_glm <- glm(Initiation ~ Sucrose.consumed + Sex + Colony, family = binomial, data = d
<br />
<br />

<p align="center">
Binomial Model - Example 2
<br/>
<img src="https://imgur.com/Kdh2Vie.png" height="80%" width="80%" />
<br />
Model call: glm(Initiation ~ Intertegular.distance..mm. + Sex + Colony, family = binomial, data = d)
<br />
<br />

<p align="center">
Binomial Model in R - Example 3
<br/>
<img src="https://imgur.com/tCP7yIp.png" height="80%" width="80%" />
<br />
Model call: glm(Initiation ~ Sucrose.consumed + Sex + Colony, family = binomial, data = d
<br />
<br />






