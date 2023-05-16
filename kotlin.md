## If/Else statement in kotlin or  conditional statements in kotlin:

thsi is also a valod block of code in Koltin

fun main() {
    val trafficLightColor = "Black"

    if (trafficLightColor == "Red") {
        println("Stop")
    } else if (trafficLightColor == "Yellow") {
        println("Slow")
    } else if (trafficLightColor == "Green") {
        println("Go")
    } else {
        println("Invalid traffic-light color")
    }

}

But to express a codeBlock with multiple conditions we use 

### Syntax:-
when (paramenter){
  condition 1 -> body 1
  condition 2 -> body 2
  condition 3 -> body 3
  condition 4 -> body 4
  
  }

### rule 1:
fun main() {
    val trafficLightColor = "Black"

    when (trafficLightColor) {
        "Red" -> println("Stop")
        "Yellow" -> println("Slow")
        "Green" -> println("Go")
        else -> println("Invalid traffic-light color")  // see this 
    }
}

### rule 2:-

comma for multiple statements (2, 3, 5, 7)

fun main() {
    val x = 3

    when (x) {
        2, 3, 5, 7 -> println("x is a prime number between 1 and 10.")
        else -> println("x isn't a prime number between 1 and 10.")
    }
}

### rule 3:

in keyword for  a range of numbers (in 1..10)

fun main() {
    val x = 3

    when (x) {
        2, 3, 5, 7 -> println("x is a prime number between 1 and 10.")
        in 1..10 -> println("x is a number between 1 and 10, but not a prime number.")
        else -> println("x isn't a prime number between 1 and 10.")
    }
}

### rule 4 :

is keyword to check datatype (is Int) 

fun main() {
    val x: Any = 20

    when (x) {
        2, 3, 5, 7 -> println("x is a prime number between 1 and 10.")
        in 1..10 -> println("x is a number between 1 and 10, but not a prime number.")
        is Int -> println("x is an integer number, but not between 1 and 10.")
        else -> println("x isn't an integer number.")
    }
}



