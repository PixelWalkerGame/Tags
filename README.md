# 🧱 Community-Driven Game Tags
Welcome to the community-driven project for improving in-game item search! This repository contains a master list of tags for the game's blocks, designed to make it easier for players to find what they're looking for within the game client.

The goal is to build a comprehensive, player-friendly search database that goes beyond the official item names. By tagging blocks with common aliases, functions, and related terms, we can make the game more accessible and enjoyable for everyone.

This project is a JSON file that our game client fetches and uses to enhance its search capabilities. Your contributions directly impact the player experience!

## 🤝 How to Contribute
We welcome all contributions, big or small. To maintain the quality and consistency of the data, please follow these guidelines when submitting a **Pull Request (PR)**.

### General Guidelines
- **Be Specific:** Tags should be directly relevant to the block. Think about what a player might type to find it.
- **Use Common Terminology:** Use aliases and terms that are widely understood by the community.
- **Alphabetical Order:** Please keep the JSON file organized alphabetically by pack name. In each pack, Foreground blocks should be alphabetized first, followed by Decoration and then Backgrounds. This makes it easier to merge changes and avoid conflicts.
- **One Block Pack Per PR:** To simplify reviews, please make a separate PR for each new or updated block pack entry.

### Contribution Process
1. Fork this repository.
2. Clone your forked repository to your local machine.
3. Create a new branch for your changes. A good naming convention is `add/block-pack-name` or `update/block-pack-name`.
4. Edit the `tags_blocks.json` file. Add or update the entry for the block you are working on.
5. Commit your changes with a clear and descriptive message (e.g., "Add tags for 'Gemstone' block pack").
6. Push your branch to your forked repository.
7. Open a Pull Request to the main repository, referencing the block you've updated.

## JSON Formatting
The `tags_blocks.json` file is a single JSON object where each key is the official [Palette Id](https://game.pixelwalker.net/listblocks) (case-sensitive) and the value is an array of strings representing the tags.
- The key (block's [Palette Id](https://game.pixelwalker.net/listblocks)) must be a string.
- The value (tags) must be an array of strings.
- Each tag within the array should be a single word.

### Correct Example:
If you wanted to add tags for the block "environment_log", a good entry would look like this:
```json
{
  "environment_log": ["Nature", "Wood", "Tree", "Brown"],
}
```
### Incorrect Examples:
- **Wrong Format:** `"environment_log": "Nature, Wood"` (This should be an array of strings.)
- **Irrelevant Tags:** `"environment_log": ["Food", "Mining", "Cool"]` (Tags must be relevant.)
- **Incorrect Key:** `"Environment_Log": [...]` (The key should match the official capitalization.)
## ❓ Questions?
If you have any questions or are unsure about a contribution, please open an Issue and we'll be happy to help!

Thank you for helping us make the game better for everyone!

\- The PixelWalker Team
