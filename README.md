## Experiment 7 – Create an Application to Demonstrate HashMap Collection Object  

<H3>ENTER YOUR NAME: J.F.SHARON ARUL BHARATHI</H3>  
<H3>ENTER YOUR REGISTER NO: 212224100056</H3>  
<H3>EX.NO.5</H3>  
<H3>DATE: 20/11/2025</H3>  

<H1 ALIGN =CENTER> Demonstrating HashMap Collection in Rust </H1>  

## AIM:  
To create a Rust application that demonstrates the use of the HashMap collection object.  

## EQUIPMENTS REQUIRED:  
- Hardware – PCs  
- Software – Visual Studio Code (Version 1.104.0)  
- Rust Installation  

## RELATED THEORETICAL CONCEPT:  

*HashMap in Rust:*  
A HashMap is a collection that stores data as key-value pairs. Keys are unique, and values can be retrieved efficiently using their associated keys.  

*Key Features of HashMap:*  
- Stores data as key-value pairs.  
- Keys must be unique, values can be duplicated.  
- Provides `.insert()` for insertion and `.get()` for retrieval.  
- Useful for fast lookups and mappings.  

## ALGORITHM:  
STEP 1: Start the program. <BR>  
STEP 2: Import `std::collections::HashMap`. <BR>  
STEP 3: Define the `main` function. <BR>  
STEP 4: Create a new HashMap to store key-value pairs. <BR>  
STEP 5: Insert values into the map using `.insert(key, value)`. <BR>  
STEP 6: Iterate and print the key-value pairs. <BR>  
STEP 7: Access values using `.get(key)` and display them. <BR>  
STEP 8: End the program. <BR>  

## PROGRAM:  



```

use std::collections::HashMap;

fn main() {
    let mut student_scores = HashMap::new();

    student_scores.insert(String::from("Alice"), 85);
    student_scores.insert(String::from("Bob"), 90);
    student_scores.insert(String::from("Charlie"), 78);
    student_scores.insert(String::from("Diana"), 92);

    println!("Student Scores:");
    for (name, score) in &student_scores {
        println!("{}: {}", name, score);
    }

    println!("\nAccessing specific student's score:");
    let student_name = "Bob";
    match student_scores.get(student_name) {
        Some(score) => println!("{}'s score is {}", student_name, score),
        None => println!("{} not found", student_name),
    }

    student_scores.insert(String::from("Alice"), 95);
    println!("\nUpdated Scores after modifying Alice's score:");
    for (name, score) in &student_scores {
        println!("{}: {}", name, score);
    }
}


```


## OUTPUT:

<img width="715" height="492" alt="image" src="https://github.com/user-attachments/assets/dac2a97b-a9c3-4078-b68b-08a978b586c7" />


## RESULT:

Thus we have succedssfully created a Rust application that demonstrates the use of the HashMap collection object.
