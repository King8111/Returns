import random as rnd
import math
# Import file containing the normal function
from normal import *

def lognormal(mean, sigma):
    y1, y2 = rnd.random(), rnd.random()
    x1, x2 = normal(y1, y2)
    # Generate random variate from a non-standard normal distribution
    v = mean + sigma * x1
    return math.exp(v)
