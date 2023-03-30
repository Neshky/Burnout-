# Burnout-from flask import Flask, render_template
import random

app = Flask(__name__)

@app.route('/')
def index():
    # Define exercises and time intervals
    exercises = ['Push-ups', 'Pull-ups', 'Shoulder press', 'Bicep curls', 'Tricep dips', 'Squats', 'Lunges', 'Deadlifts', 'Calf raises']
    set_time = 15
    rest_interval = 5
    break_time = 15

    # Generate workout data
    workout_data = {}
