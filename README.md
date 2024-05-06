# python-api-challenge
I used the AI assitant for help but only for the WeatherPy assignment. The only part I needed it was for defining the Linear regression function to plot each regression.
Here are the lines of code that the AI provided me with:

    def create_linear_regression_plot(x, y, x_label, y_label):
        slope, intercept, r_value, p_value, std_err = stats.linregress(x, y)
        fit = slope * x + intercept

        plt.scatter(x, y, color = 'blue',alpha=.1)
        plt.plot(x, fit, color='red')
        plt.xlabel(x_label)
        plt.ylabel(y_label)
        plt.annotate(f'y = {slope:.2f}x + {intercept:.2f}', (x.min(), y.min()), fontsize=15, color="red")
        print(f'The r-value is {r_value}')
