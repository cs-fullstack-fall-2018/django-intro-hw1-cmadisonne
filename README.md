# django-intro-hw1

Create a new route and paste it below. Create a blue-or-red route that takes an argument of blue or red. If it's blue, write "Sky". If it's red, write "Fire". If it's anything else write "ERROR".

Yes, I did run this in the server to check if it works... It works!

# Route
path('color/<str:userInput>/', views.blueOrRed)

# Function
def blueOrRed (request, userInput):
    if (userInput == 'blue'):
        return HttpResponse ("Sky")
    elif (userInput == 'red'):
        return HttpResponse ("Fire")
    else:
        return HttpResponse ('Error')
