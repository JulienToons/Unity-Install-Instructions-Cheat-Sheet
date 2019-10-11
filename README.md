# VR-Hackathon-10-12-19
 Our Git. Repository for whatever we do at this hackathon

## Contents:
1. ~~Create Clickup Account~~
2. Download Unity and unity collaborator extension if possible
3. Look at C# ~~vs JS~~ for Unity
4. Check out Google Maps 3D api

----

## Instructions
### 1. ~~Create a Clickup Account~~
~~Go To 
[Clickup](https://www.google.com "Google's Homepage")
 and Create an account~~
	
~~Send me (Julien) the email you used.~~

~~Once I add you, check out the board, list, and box views~~

~~Go 
[*HERE*](https://clickup.com/views)
to see an example of each view~~

~~You can use clickup online &/or download the app on your phone~~

---

### 2. Download Unity
Install Unity Hub Personal (It might say it is Unity 2019.2.4 Personal)
[*Here*](https://store.unity.com/download)
. You will need to allow the program to do whatever it needs to. 
Then Open

Next, go to installs, click ADD, and select the latest version: Unity 2019.2.8f1 Personal

Click NEXT and add the following modules:
1.	Visual Studio
2.	Android Support
3.	Windows Support
4.	WebGL Support

Click NEXT. The Program will take about **40 Min.** to install.

Once you installed Unity, open 
[the test file](testUnityGame)
 with Unity 2019 (or through Unity Hub) to make sure it installed correctly.

On the top right, go to Account and sign in to your Unity Account (make one if you havn't already)

We will decide if we will use Unity Collaborate or this Github Page on Saturday

For the VR integration we will probrably use an asset from Unity's Asset Store

### 3. Coding in Unity
Unity used to support the following languages:

| ***Language*** | **Rating** | **Description** |
| -------------- |:-------------:| -----:|
| **C#**         | THE ***BEST*** | Has alot of ready-to-use functions and is easy to learn & understand + The synatx is similar to that in Java|
| **JavaScript** | *NOT Recommended* | Less Librararies and ready to use functions & classes |
| **C++**        | For Experts Only | Allows you to program the Unity Engine itself |
| **Boo**        | Old & not recommended | Has a syntax similar to Python |
| **IronPython** | Old & not recommended | Has a syntax similar to Python |
| **Scratch**    | For Beginners | Uses Block Code similar to that in Scratch. **Dont use!**|

Now they only support C# and C++ so...

We will be using C# for Unity

---

##### C# Cheat Sheet
```C#
// It is highly recommended to start by looking up every question you have on google 

//Libraries
using UnityEngine;
using System.Collections;

public class AudioExamples : MonoBehaviour
{	
    // each global var should have the word public or private before it
    public GameObject; // GameObject is the fundemental class that every object is derived from
    /* NOTE: You dont have to set the var. in the script. Instead you can go to the untiy editor
    and drag whatever you want to the variable in the object editor (of the specific object that contains the script)
    */
    
    private AudioSource audioSource; // this is a reglar private global variable for the AudioExamples class
    // NOTE: the AudioScource class is already made by Unity. That is why C# is the best language to use here

    public static int counter = 0; // default at start if not already set in the editor
    // & yes static classes and vars exist

    // public global var
    public AudioClip clip1;
    
    // List<type> intList = new List<type>();
    public List<int> intList = new List<int>();
    
    public int[][] matrix;
/*    
// defining array with size 5. add values later on
int[] intArray1 = new int[5]; 

// defining array with size 5 and adding values at the same time
int[] intArray2 = new int[5]{1, 2, 3, 4, 5};

// defining array with 5 elements which indicates the size of an array
int[] intArray3 = {1, 2, 3, 4, 5};
*/
    
    void init(){
    	// runs once before anything else
    }
    void Start() // RECOMMENDED: runs once after init
    {
        // Get the AudioSource component from the object containing the script in the unity editor
        audioSource = GetComponent<AudioSource>();

        // Plays a function from the obj
        audioSource.Play();
	
	//
    }

    void Update() // Runs every so mseconds
    {
    	// Common methods
    	if(true){   // normal if statements
	     for(int i = 0; i<5;i++){
	     	while(true){
			break;
		}
	     }
        }
    }
    
    public void doSomething(int i){
    	// a function that can be accessed by any object, script, or editor
    }
}

// Example Class with a constructor
public class Person
{
   private string last;
   private string first;
   
   public Person(string lastName, string firstName)
   {
      last = lastName;
      first = firstName;
   }
}
```
### Check out Google Maps 3D

HERE: https://cloud.google.com/maps-platform/gaming/?utm_campaign=maps_update_googlemapsapis_040918&utm_medium=yt-desc&utm_source=gdev



