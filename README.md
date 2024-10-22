Great! Since `PyObjC` solved the issue, here's a basic structure for a `README.md` file that you can customize based on your needs:

```markdown
# Alarm Clock in Python

This is a simple Python alarm clock application that waits for a specified amount of time and then plays an alarm sound. It allows the user to input the number of minutes and seconds to wait, and when the countdown finishes, an alarm sound (`wake_up_call.mp3`) is played.

## Features

- Countdown timer that accepts user input (in minutes and seconds).
- Cross-platform terminal clearing for a clean user experience.
- Alarm sound plays once the countdown reaches zero.

## Requirements

- Python 3.x
- `playsound` library for audio playback.
- `PyObjC` for better compatibility with `playsound` on macOS.

### Install the necessary dependencies:

Run the following command to install the required libraries:

```bash
pip3 install playsound PyObjC
```

## Usage

1. **Prepare the alarm sound**: Make sure you have the `wake_up_call.mp3` file in the same directory as your script, or provide the full path to the file in the code.

2. **Run the program**:
   ```bash
   python3 basic.py
   ```

3. **Input the time**:
   - You will be prompted to enter the number of minutes and seconds to wait.
   - After entering the values, the countdown will start, and it will update in the terminal.

4. **Alarm sound**:
   - When the timer reaches zero, the `wake_up_call.mp3` file will play as the alarm.

## Example

```bash
How many minutes to wait: 1
How many seconds to wait: 30
Alarm will sound in: 01:30
Alarm will sound in: 01:29
...
Alarm will sound in: 00:00
*Alarm sound plays*
```

## Customization

- **Changing the alarm sound**: You can change the alarm sound by replacing the `wake_up_call.mp3` file with your preferred sound. Make sure to update the filename in the code if needed.
  
- **Timer functionality**: The program currently only supports input in minutes and seconds. You can modify the code to support hours if needed.

## Troubleshooting

- If you're on **macOS** and the alarm sound does not play, make sure to install the `PyObjC` package using the command:
  ```bash
  pip3 install PyObjC
  ```

- Ensure that the sound file is in the correct format (e.g., `.mp3`).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Sections to customize:
1. **Features**: You can expand this if you add more features in the future.
2. **Usage**: Adjust according to the way you run the script.
3. **Troubleshooting**: Add any other common issues you or users might encounter.
4. **License**: If you use a specific license (e.g., MIT, GPL), include a `LICENSE` file in your repository.

This `README.md` provides clear instructions, dependencies, and examples to help users get started with your alarm project!
