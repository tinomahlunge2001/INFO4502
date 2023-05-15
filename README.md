# INFO4502
# chart 1 
import pandas as pd
import plotly.express as px


df = pd.read_csv('workout_data.csv')


fig = px.parallel_categories(df, dimensions=['Duration', 'Pulse', 'Maxpulse', 'Calories'])


fig.update_layout(
    title='Workout Data',
)

fig.show()

