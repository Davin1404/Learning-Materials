# Markov

A state $S_t$ is ***Markov*** iff:  

$$P(S_{t+1}|S_t,S_{t+1},\dots,S_1)=P(S_{t+1}|S_t)\tag{1}$$  

* The states captures all relevant information from the history.  
* Once the state is known, the history may be throw away.  
* 