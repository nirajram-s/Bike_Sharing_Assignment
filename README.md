A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands

## Conclusions
- Number of Final Parameters 7
- Parameters : temp, yr, winter, Light_Snowrain,Sprint,holiday, Misty
- Train R^2 :0.808 - Train Adjusted R^2 :0.806
- Test R^2 :0.806 - Test Adjusted R^2 :0.7996

Thus we can conclude that model is fairly good and generalize various datasets and can be written as shown below
- Train R^2 and Test R^2 are almost same, similart Train Adjusted R^2 and Test Adjusted R^2 are also very close to each other
- So trained model is working with similar accuracy in test model as well
- We have reduced the number of Parameters to 7 by using RFE, p Value, VIF and our Business knowledge
cnt = 0.2082 + (temp * 0.4442) + (yr * 0.2338) + (winter * 0.0534) - (Light_snowrain * 0.2949) - (Spring * 0.1204) - (Holiday * 0.0906) - (Misty * 0.0727)

Year, Temperature, Summer, Winter, September have positive effect on the count of rental bikes
- Temperature - 0.4442
- Year - 0.2338
- Winter - 0.0534

Holiday, Windspeed, Spring, Light_snowrain and Misty have negative effect on the count of rental bikes
- Light_snowrain - -0.2949
- Spring - -0.1204
- Holiday - -0.0906
Misty - -0.0727
