# Intro To Git

Git ReadMe files and Juypiters text is written in [Markdown](https://www.markdownguide.org/cheat-sheet/), a simple markup language

### Main git Commands
- `git add` - specify which files are to be added to the repository, everything in file can be specified with "."
- `git commit -m` "commit message" - commits the changes to the local git system
- `git push` - pushes the changes to the cloud hoested Version Control on github
- `git clone repoLink` - creates a local copy of the respository in the called location

A standard set of commands when updating a repository after work is:
```bash
  git add .
  git commit -m "specify changes made"
  git push
```

## Python best Practices
### Using a Virtual Enviroment 
The use of a virtual enviroment in python is good for encapluating code, it allows you to store the libraries used with the code so that when a project is run on another computer you dont need to reinstall all used libraries.

To create a virtual enviroment navigate to the project directory and run the terminal command `python3 venv enviromentName`

To activate the virual enviroment naviagate to the home directory and run the terminal command `enviromentName/Scripts/activate`


## Jutpiter Notebook
### Finding Datasets
- [Kaggle](https://www.kaggle.com/datasets)



To show that the sample mean of the continuous random variable X converges to the expected value of X, which is $\frac{1}{3}$, as the sample size $n$ goes to infinity, we can use the law of large numbers.

Recall that the sample mean of $n$ observations of $X$ is defined as:

$$\overline{X} = \frac{X_1 + X_2 + \cdots + X_n}{n},$$

where $X_1, X_2, \ldots, X_n$ are i.i.d. random variables with the same distribution as $X$.

According to the law of large numbers, as the sample size $n$ increases, the sample mean $\overline{X}$ converges in probability to the expected value $\mu$ of $X$, which is $\frac{1}{3}$. Formally, we can state this as follows:

For any $\varepsilon > 0$, we want to show that:

$$\lim_{n\to\infty} \mathbb{P}(|\overline{X} - \mu| \geq \varepsilon) = 0,$$

where $\mu = \mathbb{E}(X) = \frac{1}{3}$.

To prove this, we can use Chebyshev's inequality, which states that for any random variable $X$ with finite expected value $\mu$ and finite variance $\sigma^2$, and for any $\varepsilon > 0$,

$$\mathbb{P}(|X - \mu| \geq \varepsilon) \leq \frac{\sigma^2}{\varepsilon^2}.$$

Applying Chebyshev's inequality to $\overline{X}$, we get:

$$\mathbb{P}(|\overline{X} - \mu| \geq \varepsilon) \leq \frac{\operatorname{Var}(X)}{n\varepsilon^2}.$$

Since the PDF of $X$ is $f(x) = 8x$, we can compute the expected value and variance of $X$ as follows:

$$\mathbb{E}(X) = \int_{0}^{1/2} x f(x) dx = \int_{0}^{1/2} 8x^2 dx = \frac{1}{3},$$

$$\mathbb{E}(X^2) = \int_{0}^{1/2} x^2 f(x) dx = \int_{0}^{1/2} 8x^3 dx = \frac{1}{8},$$

$$\operatorname{Var}(X) = \mathbb{E}(X^2) - [\mathbb{E}(X)]^2 = \frac{1}{8} - \left(\frac{1}{3}\right)^2 = \frac{7}{72}.$$

Substituting these values into the inequality, we get:

$$\mathbb{P}(|\overline{X} - 1/3| \geq \varepsilon) \leq \frac{7/72}{n\varepsilon^2}.$$

To show that $\lim_{n\to\infty} \mathbb{P}(|\overline{X} - 1/3| \geq \varepsilon) = 0$, we can take the limit of both sides of the inequality as $n$ goes to infinity:
