# Final Project

This will be a project done in groups of 2 or 3 to create a game with **graphics** and **animations** using **JavaFX**.

Here are a few project ideas: Brickbreaker, Ballz, Stack, Tetris, Snake, Pikes (or other simple io games), Connect 4, Battleship, Frogger, Space Invaders, a Tower Defense Game, a Super Mario level, a simple Pokemon clone, Minesweeper, Blackjack, Solitaire.

Feel free to come up with your own idea. Just remember you must be able to create
it with a graphical user interface and it must have animations. Please get your
idea approved by Mr. King before starting.

## Project Rubric

I will be scoring your project based on the rubric below and it is 7% of your final grade.

| Scoring Rubric | 6                                          | 4         | 1       |
| -------------- |------------------------------------------- | --------- |-------- |
| Code Style     | Good indentation and braces; easy to read with comments for each method. Multiple classes are used to organize code logic (no major logic done in `main`.) | Pretty easy to read, occasional error with indentation or braces, comments lacking. | Not easy to read, style conventions are not followed. |
| Functionality  | Program compiles and executes according to specifications. | Program compiles, but a few details of the specification have not been met. | Program does not compile and/or does not achieve desired results according to specifications. |
| Robustness     | Edge cases are accounted for; no unexpected execution (negative length/weight, etc.). | Not all edge cases are accounted for, but no major consequences result. | None or very few of the edge cases have been considered and cause issues with the program. |
| Collaboration  | All teams members contribute code to the project and work well as a team. | All team members contribute code, but distribution may be uneven and/or team members have trouble agreeing on ideas. | Distribution of work is severely uneven and/or team members struggle to agree on ideas. |

**All team members should be working on the code, not just watching one person code.**

**Codeshare.io is an online editor that everyone can edit at the same time like Google Docs. Github is a good place to keep "master" files for people to edit, although it is not a live editor like Codeshare or Google Docs.**

## Submission

Please have Mr. King run your code before turning it in. Make sure you have tested it thoroughly because he will find a way to break it, if possible!

At the top of your Runner class file put the team members' first and last names and give a brief explanation of what they did to contribute to the project and code.

Please have **ONE** team member submit the project to Google Classroom.

## Helpful Code

### Sounds

```
import javafx.scene.media.Media;
import javafx.scene.media.MediaPlayer;
import java.io.File;

String musicFile = "StayTheNight.mp3";     // For example
Media sound = new Media(new File(musicFile).toURI().toString());
MediaPlayer mediaPlayer = new MediaPlayer(sound);
mediaPlayer.play();
```

### Images

```
import javafx.scene.image.Image;
String filePath = "image_name.png";
Image image = new Image(getClass().getResourceAsStream(filePath));
gc.drawImage(image, 100, 200);
```

### Rotate Object

```
double rotationCenterX = (x + w / 2);
double rotationCenterY = (y + h / 2);

gc.save();
gc.translate(rotationCenterX, rotationCenterY);
gc.rotate(deg);
gc.translate(-rotationCenterX, -rotationCenterY);

gc.fillRect(x, y, w, h);
gc.restore();
```


