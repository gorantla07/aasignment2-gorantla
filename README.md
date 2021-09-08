# aasignment2-gorantla
Creating a new repository for the assignment 2.
# Manoj Gorantla
###### New York City
New York City is the largest city in the Unites states. New York City is the hub for the **Finance, Business, and Education** It has many tourist attrcations like **Times Square and Wall Street**

### Travel Insturctions...

---

1. From your location i.e., Brooklyn, New York take a taxi to the JFK International Airport.
    1. Board a Flight to the Kansas City from NYC.
    2. From a Kansas city get a Taxi and go to the Kansas City Bus Station.
2. From Kansas City Bus Station board a Bus to the Maryville, Missouri.
    1. From Maryville, Missouri downtown go starigt towards North untill you reach Finish Line.
    2. From Finish Line go towards East continue on the 7th street untill you reach Parkway Terrace Apartments.

+ From Maryville bring lots of Food and Drinks to the NYC.
    + Solid Food
        + Rice.
        + Curries
        + Yogurt
    + Beverages
        + Diet COke
        + Bud Light

[View AboutMe](AboutMe.md)

### Dinning Menu...

---

| Drinks     | Location  | Amount   |
| -----------|   --------|   -------|
|Diet Coke   | Colden Hal| $1.10    |
|Diet Pepsi  | Valk Build| $1.05    |
|Dr. Pepper  | Garret str| $1.08    |

### Best Quotes...

---

> Without Begining, no one can taste fail and no one can taste successfull
>***APJ Kalam***

> If you don't ask, you won't get it.
>***M.K.Gandhi***

### Code Fencing,,,

---

> Very few theoretical results have been obtained to date about the behavior of information retrieval algorithms under random deletions, as, well as random insertions.<br>
> A step-by-step expository analysis of this problem is given, and it is shown how the difficulties arise and can be surmounted.

Formal definition can be represented in the following elementary O(n2) implementation.

```

vector<int> z_function_trivial(string s) {
    int n = (int) s.length();
    vector<int> z(n);
    for (int i = 1; i < n; ++i)
        while (i + z[i] < n && s[z[i]] == s[i + z[i]])
            ++z[i];
    return z;
}
vector<int> z_function(string s) {
    int n = (int) s.length();
    vector<int> z(n);
    for (int i = 1, l = 0, r = 0; i < n; ++i) {
        if (i <= r)
            z[i] = min (r - i + 1, z[i - l]);
        while (i + z[i] < n && s[z[i]] == s[i + z[i]])
            ++z[i];
        if (i + z[i] - 1 > r)
            l = i, r = i + z[i] - 1;
    }
    return z;
}

```
<https://www.sciencedirect.com/science/article/pii/002200007890020X>


