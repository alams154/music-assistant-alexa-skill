# Music Assistant Alexa Skill

This project is an Alexa skill that integrates with [Music Assistant](https://music-assistant.io/) to provide audio playback using the AudioPlayer interface. The skill fetches the latest stream URL from your Music Assistant instance and plays it on Alexa-enabled devices.

## Features

- Voice control for starting, pausing, and resuming playback of your Music Assistant audio stream.
- Uses the AudioPlayer interface for seamless background playback.
- Customizable to your own Music Assistant server and API.

## Skill Architecture

The skill consists of an inteface model and logic of the skill. This skill plays a single audio stream,
along with handlers for all of the AudioPlayer events, touch controls and error handling.

### Documentation

#### Importing the Skill from a Git Repository

You can import this skill into the Alexa Developer Console using the Git repository:

1. Go to the [Alexa Developer Console](https://developer.amazon.com/alexa/console/ask).
2. Click **Create Skill**.
3. Enter a skill name and choose your default language.
4. Select **Music & Audio** as the experience, **Custom** as the model, and **Alexa-Hosted (Node.js)** as the hosting service.
5. Click **Import skill** and enter **<https://github.com/alams154/music-assistant-alexa-skill.git>**.
6. Wait for the import process to complete. The code and resources from the repository will be available in your skill project.

For more details, see the [official documentation](https://developer.amazon.com/docs/alexa/hosted-skills/alexa-hosted-skills-git-import.html).

#### Customize and Build the Skill

1. Go to the **Build** tab in the Alexa Developer Console.
2. Click the **Invocation Name** field and type in **music assistant** and hit save
3. Go to the **Code** tab and open the `index.js` file.
4. Change the **API_HOSTNAME** and **MA_HOSTNAME** constants to point to your API and Music Assistant instance.
5. Change the **API_USERNAME** and **API_PASSWORD** constants regarding the basic auth settings of the alexa api container or your reverse proxy.
6. Click **Deploy** to deploy the skill
7. Go to the **Test** and enable skill testing in **Development**
8. Go to the **Build** tab and build the skill
