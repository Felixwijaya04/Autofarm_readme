### Autofarm

![image](https://github.com/Felixwijaya04/Autofarm_readme/blob/main/images/Gif_Autofarm.gif)

## 🔴About Game
**Autofarm** is an educational puzzle game about learning how to arrange a pseudocode. The game is intenteded for audience who want to start their programming journey. In this game, player will plays as a last person who can save humanity from polutions by searching a single plant in the universe. The game consist of several different levels and objective with each difficulty.

## 📋 Project Info

<b> Developed with Unity 2022 </b>

| **Role** | **Name** | **Development Time** 
|:-|:-|:-|
| Game Programmer | Felix Wijaya | 1 month |
| Game Designer | Felix Wijaya | 1 week |
| 2D Artist & Animator | Vincent Tanujaya | 1 month |

<details>
  <summary> <b>My Contribution (Game programmer)</b> </summary>
  
  - Core mechanics
  - UI Navigation
  - Cutscene 

</details>
<details>
  <summary> <b>My Contribution (Game designer)</b> </summary>
  
  - Game mechanics
  - Level design
  - Core loop

</details>

## 📜 Scripts

|  Script       | Description                                                  |
| ------------------- | ------------------------------------------------------------ |
| `Compiler.cs` | Responsible for checking answers by comparing it from `LevelMaker.cs` |
| `LevelMaker.cs`  | Allowing developers to create a new level design |
| `FunctionLogic`  | A folder containing all function identity such as `Plant.cs`, `Loop.cs` etc |
| `UI_Manager.cs`  | Controls UI navigation |
| `ObjectControl.cs` | Manages the logic for drag and drop the code block |

<br>

## 🔥Development Process
- **Drag and Drop** <br> Our main game mechanic is drag and drop a code block. Player drags the code block from the code list then drop it in the corresponding code slot. To make a drag and drop features, we use grid layout group to create a slots for each type of code. Then we do the same thing to the code slot but vertically.
![image](https://github.com/Felixwijaya04/Autofarm_readme/blob/main/images/Screenshot%202024-10-08%20201441.png)
<br>When player hold and drag one of the code logo, the game will instantiate a corresponding code block. The code block can only be placed inside the code slot area otherwise the code block will be deleted. Player can delete a code block that has been placed inside the slot by drag and drop it outside the area.
- **Compiler** <br> To check whether the answers are correct, we created a custom compiler inside the game that will check each line of code and the text input in each code block. First, we create 2 list to contain the code type and the text input in every code block. Then we verify whether the first line of the code is attach by a correct code and text input.<br>
![image](https://github.com/Felixwijaya04/Autofarm_readme/blob/main/images/Screenshot%202024-10-08%20203105.png)
<br>If every line of codes are correct then the game will advance to the next level. Moreover, the game will play an animation if the compiler return true or false based on the answer submitted.
- **Cutscene Animation** <br> As the game begins, players are treated to an immediate short cutscene animation. Behind the scenes, we’ve employed a timeline sequence to create the cutscene. We use timeline instead of animation because timeline is more suitable for controlling multiple objects in sequence and is commonly used for creating cutscene. Meanwhile animation is best used for isolated things such as character animation.
![image](https://github.com/Felixwijaya04/Autofarm_readme/blob/main/images/Screenshot%202024-10-08%20200819.png)
