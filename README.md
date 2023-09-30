# tesla
# Assuming you have already loaded Tesla stock data into tesla_data

# Reset the index
tesla_data.reset_index(inplace=True)

# Display the first five rows
print(tesla_data.head())

# Assuming you have a DataFrame named 'tesla_revenue_data' with revenue data
# Make sure you have already scraped and loaded the data into the DataFrame

# Display the last five rows
print(tesla_revenue_data.tail())

# Assuming you have already loaded stock data for GM into the 'gmedata' DataFrame

# Reset the index
gmedata.reset_index(inplace=True)

# Display the first five rows
print(gmedata.head())

# Assuming you have a DataFrame named 'gme_revenue_data' with revenue data for GameStop
# Make sure you have already scraped and loaded the data into the DataFrame

# Display the last five rows
print(gme_revenue_data.tail())

import matplotlib.pyplot as plt

# Assuming you have Tesla stock data in the 'tesla_data' DataFrame
# Replace 'tesla_data' with the actual DataFrame containing Tesla stock data

def make_graph(data, title):
    plt.figure(figsize=(12, 6))
    plt.plot(data['Date'], data['Close'], label='Closing Price', color='blue')
    plt.title(title)
    plt.xlabel('Date')
    plt.ylabel('Closing Price')
    plt.legend()
    plt.grid(True)

# Provide a title for the graph
graph_title = "Tesla Stock Price Over Time"

# Call the make_graph function to plot the data
make_graph(tesla_data, graph_title)

# Display the graph
plt.show()
