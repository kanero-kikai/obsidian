- The **learning rate** is a tuning parameter in an optimization algorithm that determines the **step size** at each iteration while moving toward a minimum of a cost function.
- It metaphorically represents the speed at which a machine learning model "learns".
- And also represents the size of the parameters update.
## Learning Rate Impact on Learning
If the learning rate is **Too small**, The algorithm **will Work**, but **very Slow**, as it's taking very small steps. 
![[Gradient Descent-20240610105745969.png|218]]
If the learning rate is **Too Large**, It will take huge steps that will **get bigger and bigger by time**. And the cost function will increase. And the model will **not converge**, it may even diverge.    
![[Gradient Descent-20240610105805281.png|218]]
