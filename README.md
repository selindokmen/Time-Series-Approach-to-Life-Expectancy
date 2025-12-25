# Time-Series-Approach-to-Life-Expectancy
Life Expectancy in Germany: a time-series approach. Using WorldBank dataset, life expectancy of Germany has been explored.

Introduction
This project aims to analyze the life expectancy trends of the country Germany over the years of 1960 to 2023. Life expectancy is a metric that is greatly influencial on the well-being and socio-economic norms of a nation and is important to be analyzed and worked on to improve. World Development Indicators bulk dataset has been used from The World Bank website and data of Germany has been preprocessed in order to serve the purpose of our project. The time-series data has been analyzed in two-approaches: univariate and multi-variate analysis. Exploratory Data Analysis has been applied to the data first, and then the data is analyzed by means of time-series.

The work progressed in several stages. Exploratory
Data Analysis confirmed that life expectancy in Germany has increased steadily and almost monotonically since 1960, with only minor fluctuations. After
preprocessing the dataset, two modeling strategies
were adopted: (i) univariate time-series forecasting
models and (ii) multivariate extensions that included
socioeconomic variables.
Univariate modeling was carried out using ARIMA.
This provided a reliable benchmark, showing that life
expectancy could be forecast with high accuracy by relying on its own past values. The error metrics confirmed this: RMSE was approximately 0.25 years and
MAPE was just 0.26%, demonstrating that the forecasts were extremely close to the observed values.
Multivariate modeling with SARIMAX extended this
approach by including external regressors such as
GDP per capita, infant mortality, and fertility rate. In
this framework, GDP per capita was found to have
a positive and statistically significant impact on life
expectancy, while infant mortality had a strong negative effect. Fertility rate did not contribute significantly. These results align with expectations from
demographic and economic theory: improvements in
economic prosperity and reductions in infant mortality
are closely linked to rising life expectancy. The SARIMAX model therefore allowed us to quantify how socioeconomic factors co-move with health outcomes,
while still delivering accurate forecasts.
True multivariate modeling was implemented
through a VAR specification, which treated life expectancy, GDP per capita, infant mortality, and fertility
rate jointly. The results indicated that life expectancy
is primarily explained by its own lagged values, reflecting its persistent and stable upward trajectory. GDP
per capita, however, was influenced not only by its own
past but also by lagged life expectancy, suggesting
that demographic improvements can have delayed effects on economic performance. Infant mortality and
fertility rate were mostly autoregressive, with their dynamics dominated by their own histories.
Taken together, these findings reveal a coherent story.
Life expectancy in Germany has followed a strong upward trend for decades, largely explained by its past
trajectory but also closely associated with key socioeconomic variables. The fact that GDP per capita and
infant mortality emerge as significant determinants
highlights the interplay between public health and
economic development. From a forecasting perspective, both ARIMA and SARIMAX produced highly accurate results, while VAR provided additional insights
into the interdependencies between variables.
The project demonstrates that combining univariate
forecasting, regression with exogenous drivers, and
multivariate system modeling yields a richer understanding of demographic dynamics. For policymakers,
such analysis is valuable because it shows not only
that life expectancy can be forecast with precision, but
also that improvements in economic well-being and
reductions in infant mortality are essential levers for
further progress.
Future research could extend this work by including
additional variables such as healthcare expenditure,
education levels, or environmental indicators. Moreover, experimenting with machine learning–based
forecasting methods could complement classical statistical models and provide robustness under structural shifts.
In conclusion, the study confirms that life expectancy
in Germany is on a stable upward path, driven by longterm demographic momentum and reinforced by socioeconomic progress. Statistical modeling has not
only provided precise forecasts but also shed light on
the broader determinants of health, offering evidencebased insights that can guide social and economic policy.
