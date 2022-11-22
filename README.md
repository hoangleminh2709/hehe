// Q1- print to the screen even numbers from 1 to 10
for (let i = 1; i <= 10; i++){
    if( i % 2 == 0){
        console.log (i);
    }
}

// Q2 - using if else  and while to Check prime number.
// input: 5
// output: True
var n = (5)
let isPrime = true;
if (n === 1) {
    console.log(false);
}

else if (n > 1) {
    for (let i = 2; i < n; i++) {
        if (n % i == 0) {
            isPrime = false;
            break;
        }
    }

    if (isPrime) {
        console.log(true);
    } else {
        console.log(false);
    }
}

else {
    console.log(false);
}
    


// Q3-sort the following array in ascending order using loop
// input: [2,1,7,2,6,9,1,99,12,56]
// output:[1,1,2,2,6,7,9,12,56,99]
var myArray = [2, 1, 7, 2, 6, 9, 1, 99, 12, 56];

for (var i = 1; i < myArray.length; i++)
    for (var j = 0; j < i; j++)
        if (myArray[i] < myArray[j]) {
          var x = myArray[i];
          myArray[i] = myArray[j];
          myArray[j] = x;
        }

console.log(myArray);


// Q4 - sort the following array in descending order using loop
// input: [2,1,7,2,6,9,1,99,12,56]
// output:[99,56,12,9,7,6,2,2,1,1]
var myArray = [2, 1, 7, 2, 6, 9, 1, 99, 12, 56];

for (var a = 1; a < myArray.length; a++)
    for (var b = 0; b < a; b++)
        if (myArray[a] > myArray[b]) {
          var z = myArray[a];
          myArray[a] = myArray[b];
          myArray[b] = z;
        }


// Q5-  Given a string is the path of a file in the computer. The correct path is a path that has no leading and trailing slashes (/) and only one slash in between folders to separate it. Please remove the extra slashes to get a correct path
// input:  ////laptrinh//////code//////javascript/////
// output: laptrinh/code/javascript
