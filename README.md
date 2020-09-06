# skinfetch
Discord bot that fetches the skin file of any Minecraft profile.

When the user enters a command like !skin Dinnerbone, the bot will fetch information from https://api.mojang.com/users/profiles/minecraft/Dinnerbone to get the UUID of that user. Then, it will get information from properties/value on https://sessionserver.mojang.com/session/minecraft/profile/61699b2ed3274a019f1e0ea8c3f06bc6. Then, it will take this base64 value and decode it. Then, using the URL under textures/SKIN/url, it will enlarge the skin file and send it in the Discord server where the message was sent.
