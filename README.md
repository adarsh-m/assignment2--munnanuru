# assignment2--munnanuru
# Adarsh Munnanuru
###### Goa
>Goa is a state in western **India** with coastlines stretching along the **Arabian Sea**. Its long history as a **Portuguese** colony prior to >1961 is evident in its preserved 17th-century churches and the area’s tropical spice plantations. Goa is also known for its beaches, >ranging from popular stretches at Baga and Palolem to those in laid-back fishing villages such as Agonda.
***
# Directions to Maryville to Kansas
1. Start from the source
2. Take via Local road
    1. Take first left
    2. Then take second right towards the free way
1. Take via free way
2. Drive until Kansas

* Items to be taken for the trip
    * Barbeque
    * camp tent
    * fan
    * powerbank
    * balls

**[My Profile](AboutMe.md)**

 ---
 # Recommended Foods - Barbecue and Beyond
Sunday dinners, potluck gatherings and farmhouse meals feature prominently among the foods that inspire the people in this middle-of-the-U.S. state. A state wealthy in farmland and cattle ranches is sure to serve some good food. So, come “Home on the Range” with the comfort foods of Kansas.

Food/Drink | Location | Price
--- | --- | ---
Chicken Biryani | Godavari | $22
Steak | Hot Wox | 40$

---

# Quotes
> "The purpose of our lives is to be happy."
> *— Dalai Lama*

> “Life is what happens when you’re busy making other plans.” 
> *— John Lennon*
---
# String Processing
>String hashing is the way to convert a string into an integer known as a hash of that string.
An ideal hashing is the one in which there are minimum chances of collision (i.e 2 different strings having the same hash). (https://www.geeksforgeeks.org/string-hashing-using-polynomial-rolling-hash-function)

```
long long compute_hash(string const& s) {
    const int p = 31;
    const int m = 1e9 + 9;
    long long hash_value = 0;
    long long p_pow = 1;
    for (char c : s) {
        hash_value = (hash_value + (c - 'a' + 1) * p_pow) % m;
        p_pow = (p_pow * p) % m;
    }
    return hash_value;
}

```

[source code](https://cp-algorithms.com/string/string-hashing.html)