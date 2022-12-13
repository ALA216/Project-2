# Project 2: SIR model parameter estimation for COVID-19 spread in Italy most affected city [Lombordia]

With four parameters I can fit an elephant, and with five I can make him wiggle his trunk” – Johnny Von Neumann.
The phrase "With four parameters I can fit an elephant, and with five I can make him wiggle his trunk" is a humorous way of expressing the idea that complex data can often be fit well by simple models, but those additional parameters can be used to fine-tune the model and make it more accurate. This is a common issue in statistics and data analysis, where it is often tempting to use more and more parameters in an attempt perfectly fit the data. However, this can occasionally leads to overfitting, in which the model becomes so complex that it does not generalize well to new data.
The SIR model is a type of mathematical model that is commonly used to study the spread of infectious diseases. It is an epidemiological model that categorizes a population as susceptible, infected, and recovered. The SIR model tracks the flow of individuals between these three states over time, based on certain assumptions and parameters, such as the transmission rate of the disease and the rate at which people recover from it.
One way to extend the SIR model to include death is to add a fourth state for individuals who have died from the disease. This modified SIR model (called the SIR-D model) would monitor the flow of individuals between the four states: susceptible, infected, recovered, and dead. The transmission rate, recovery rate, and death rate would be used to calculate the flow of individuals between these states over time. Overall, the SIR-D model can be a useful tool for studying the spread of infectious diseases, such as COVID-19, and for predicting the potential impact of various public health interventions. However, it is important to note that all mathematical models are simplifications of reality, and the results they produce should be interpreted with caution and in the context of other relevant information.

## Application

The SIR-D model can be a useful tool for policymakers and public health officials to study the spread of infectious diseases such as COVID-19, and to evaluate the potential impact of different interventions. For example, the model can be used to predict the potential impact of implementing a vaccination program or implementing social distancing measures on the spread of the disease.
By inputting different values for the transmission rate, recovery rate, and death rate into the SIR-D model equations, and by assuming certain values for the initial number of susceptible, infected, recovered, and dead individuals in the population, it is possible to generate predictions of the future course of the disease under different scenarios. These predictions can then be used to inform decision-making and to evaluate the potential effectiveness of different policy interventions.
Overall, the SIR-D model has the potential to be a useful tool for studying the spread of infectious diseases.

## Mathematical Model

The SIR-D model is a set of differential equations that describe the flow of individuals between the four states (susceptible, infected, recovered, and dead) over time. The equations are as follows:

 where:

- S is the number of susceptile individuals
- I is the number of infected individuals
- R is the number of recovered individuals
- D is the number of dead individuals
- N is the total population size
- beta denotes the transmission rate of the disease (the rate at which susceptible individuals become infected)
- gamma denotes the recovery rate (the rate at which infected individuals recover)
- mu denotes the death rate (the rate at which infected individuals die)
- dS/dt, dI/dt, dR/dt, and dD/dt are the rates of change of the respective populations over time
These equations can be used to model the spread of an infectious disease in a population and to predict the potential impact of different interventions. However, as mentioned earlier, it is important to remember that these equations are simplifications of reality, and the results they produce should be interpreted with caution.

## Data
Data is obtained from Italy most affected region Lombordia.
 ![image](https://user-images.githubusercontent.com/112144648/207378491-0213e920-4b98-4c10-9c20-ff6e786e3713.png)
![image](https://user-images.githubusercontent.com/112144648/207378564-988999a6-3264-4510-96f6-452e5ef7369d.png)
![image](https://user-images.githubusercontent.com/112144648/207378619-aaa602fe-84db-4f98-aa8f-df8d605f88ce.png)
Figure 1 shows the study effect of death rate, disease rate/infection rate over the population with passage of time.

## Sensitivity Analysis
In order to analyze the sensitivity of a system to changes in its parameters, we can perturb the parameters multiple times over a broad range of values. It is important to choose a range that is meaningful for the specific system and question we are trying to answer.
Once we have chosen our range, we can run the system's equations (odes) for each parameter set and collect the output. We can then fit the output to a linear model in order to estimate the sensitivity of the system to changes in the parameters.
The choice of output (i.e. the steady state value, maximum over time, area under the curve, etc.) will depend on the specific question we are trying to answer. For example, if we are interested in the maximum response of the system to a perturbation, we may choose to use the maximum value over time as our output.
Why use a linear model? By using a linear model, we can easily estimate the sensitivities of the system by applying least squares regression. This allows us to determine how sensitive the system is to changes in each of its parameters.
![image](https://user-images.githubusercontent.com/112144648/207379682-ae063e7b-05a2-4c9c-abd4-68450430c0a8.png)
![image](https://user-images.githubusercontent.com/112144648/207379580-6cac43d2-703b-49a5-8d9d-04aa12b9c5fa.png)
## Bifurcation Analysis
A bifurcation diagram is a visual tool used to analyze the behavior of a system, such as the SIR model, as a parameter (such as the infection rate) is varied. The diagram shows how the steady states of the system change as the parameter is changed, allowing for insight into the dynamics of disease transmission and the effectiveness of interventions. Bifurcation diagrams are useful for understanding the behavior of simple first order systems, but their application is limited by our ability to visualize complex systems.
![image](https://user-images.githubusercontent.com/112144648/207380176-764f6a60-b562-47b3-99ad-ee63cd5ddda8.png)
