# Ex.No: 3  Basic movements in Unity 
### DATE: 28/04/2025                                                                            
### REGISTER NUMBER : 212224220010
### AIM: 
 To learn the basic movements translation,scaling and rotation of game objects through code.
### Procedure:
1. Setup the Scene
2. Open Unity and create a 3D Scene.
3. Add three objects:Cube → Rename to Object1 (for movement),Sphere → Rename to Object2 (for rotation).Capsule → Rename to Object3 (for scaling).
4. Add the Script,Create a C# Script → Name it TransformOperations.cs.
5. Write the code for translation,scaling and rotation,save and close the script
6. Save the script
7. Select any empty GameObject (or create one: GameObject → Create Empty).
8. Attach the TransformOperations script to it.
9. In the Inspector, assign Object1 → Drag the Cube,Object2 → Drag the Sphere.Object3 → Drag the Capsule.
10. Run the Scene Press Play ▶️ in Unity
11. Stop the program.
### Program 
```
 using UnityEngine;

public class firstscript : MonoBehaviour
{
    // Start is called once before the first execution of Update after the MonoBehaviour is created
    public Transform o1;
    public Transform o2;
    public Transform o3;
   
    void Start()
    {


    }

    // Update is called once per frame
    void Update()
    {
        if (Input.GetKeyUp(KeyCode.X))
        {
            o1.Translate(1f, 0, 0);
        }
        if (Input.GetKeyUp(KeyCode.Y))
        {
            o2.Rotate(20f, 0, 0);
        }
        if (Input.GetKeyUp(KeyCode.Z))
        {
            o3.localScale += new Vector3(0, 0.2f, 0);
        }
    }
}
```
### Output:


<img width="1253" height="662" alt="Screenshot 2026-04-28 142124" src="https://github.com/user-attachments/assets/ba96071c-9fb3-4ce9-b114-4c7160b7c921" />






### Result:
Thus the basic movement is learned through scripting


