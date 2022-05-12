# quant-systems

Trading systems using quantitative methods.


The goal of this project/research is to optimize a technical trading strategy using machine learning techniques. The process
will consist of developing a trading strategy, mining the data, backtesting, optimizing the trading signals using machine learning, 
and then backtesting again. We will compare the results of the optimized strategy with the initial strategy and come to a conclusion if
the machine learning techniques imporved our models.

Out trading strategy will consist of several indicators that will lead to an if-then decision. As a base model, we will be
using an adaptive moving average of a modified ATR. This will allow us to formulaize the contraction and expansion of price. 
This will be fed into a trailng stop line, if price crosses above the line, we long (buy), if price crosses below the line, we
short (sell). Again, this is a base strategy, more indicatorts will be added on in the cycle of development. 

We will then backtest the base strategy and asses its viability. If it is viable, we will mine the data. Meaning every long and 
short signal will be logged. We will split this data into training and testing sets. With the data properly prepared, will run 
several machine learning models, such as Linear Model, Artificial Neural Networks, Random Forest, and Support Vector Machine/Regression.
The research work used as a reference for this work is from https://doi.org/10.1016/j.knosys.2021.107119. The models will be assed for
precision, accuracy, and other metrics. After finding an optimal model, we will feed this back into our trading strategy, where the signals
are now refined, and backtested again. This cycle can repeat as long as there signs of improvement. There are still decisions and unknowns to be
made such as the exact design of the machine learning models, whether we will orrient the problem as a regression or classification problem. These
unkowns will be worked out as we continue forward with this work. 

