Geiger counter: radiationDv1.1 cajoe

signal comes from misslabled vin port

Its a falling signal, should be interrupt based, will start with polling first

we should at first figure out what pin can accept such a signal that fast. 1 second is 1 million microseconds

we do it via vin pin on the geinger counter.



the question is..what pin on the micro controller?

i think its good to power the device using the micro controller. so we gotta figure out how to get 5v rail enabled


ok now we are flashing but i want to instead read input from a pin */
I beleive the signal is digital so we need to mess with a digital pin */
we must turn it on*/
we will poll it for signal */
4.747v from my bm245 */
drops by 600 mv for 700micro secconds too fast for my multimeter */


