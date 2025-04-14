# Automated-welcoming-message
# Example pseudo-code
import dotbot_api

# Authenticate
bot = dotbot_api.authenticate("your_api_key")

# Fetch new nations
new_nations = bot.get_new_nations(region="The Fries")

# Construct the message
message = "Welcome to our region! 🎉 We are excited to have you here, @" + ", @".join(new_nations)

# Post to the regional message board
bot.post_message(region="The Fries
", message=message)
