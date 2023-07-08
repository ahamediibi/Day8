# Day8

Day 07: ARRAY METHODS

1,Solving problems using array functions on the rest countries' data:
Question: Perform various tasks using array functions on the data retrieved from the "restcountries.com" API.
Answers:
a. Get all the countries from the Asia continent/region using the Filter function

const asiaCountries = countries.filter(country => country.region === "Asia");
console.log(asiaCountries);

b. Get all the countries with a population of less than 2 lakhs using the Filter function:

const countriesWithLowPopulation = countries.filter(country => country.population < 200000);
console.log(countriesWithLowPopulation);

c. Print the name, capital, and flag of each country using the forEach function:

countries.forEach(country => {
  console.log("Name:", country.name);
  console.log("Capital:", country.capital);
  console.log("Flag:", country.flag);
});

d. Calculate and print the total population of all countries using the reduce function:

const totalPopulation = countries.reduce((acc, country) => acc + country.population, 0);
console.log("Total Population:", totalPopulation);

e. Find and print the country that uses US Dollars as currency using the find function:

const countryWithUSD = countries.find(country => country.currencies.includes("USD"));
console.log(countryWithUSD);
