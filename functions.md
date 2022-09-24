1. Do the below programs in anonymous function & IIFE:
------------------------------------------------------

(a) Print odd numbers in an array.
==================================
(function(a){for(var i=0;i<a.length;i++)if(a[i]%2!=0)console.log(a[i]);})([1,2,3,4,5,6,7]);


*********************************************************************************

(b) Convert all the strings to title caps in a string array
===========================================================
var arr=["apple","beetroot","carrot","drumstick","eggplant","fig"];
(function(arr){for(var i=0;i<arr.length;i++)console.log(arr[i][0].toUpperCase()+arr[i].substr(1))
})(arr);

*********************************************************************************

(c) Sum of all numbers in an arry
=================================
var s=0;
(function(arr){for(var i=0;i<arr.length;i++)s=s+arr[i];console.log("Sum of array is:"+s)})([1,2,3,4,5]);

*********************************************************************************


(e) Return all the palindromes in an array
==========================================
var temp=[];
(function(a){for(var i=0;i<a.length;i++)
{var rev=a[i].split("").reverse().join("");
if(a[i]===rev)
temp.push(a[i]); }
     console.log(temp);})(["geek","mam","lol"])
	 
*********************************************************************************

(f) Return median of two sorted arrays of the same size
=======================================================
(function(a,b){var c=a.concat(b)//merging a,b array and store in c
var mid = Math.floor(c.length / 2)//finding the avg of array c length,foor rounddown the mid
//console.log('mid : ', c[mid]);
var midval=c[mid]+c[mid-1];
return console.log("Median : "+midval)//13
})([1,2,3,4,5,6],[7,8,9,10,11,12])

*********************************************************************************

(g) Remove duplicates from an array 
=====================================

(function(a){for(var i=0;i<a.length;i++)
if(a[i]===a[i+1])//comparing element of a, to find the duplicates
a.splice(i+1, 1);//if yes remove the duplicate
console.log(a)//[ 'a', 'b', 'c', 'A', 'd' ]
})(['a','b','c','A','d','d'])



*********************************************************************************

(h) Rotate an array by k times
==============================
(function (a){
  var k=3;for(var i=0;i<=k;i++)

  a.unshift(a.pop());return console.log(a)})( [1,2,3,4,5]);

*********************************************************************************

----------------------------------------
Do the below program in arrow functions:
----------------------------------------

(a) Print odd numbers in an array.
==================================
var a=[1,2,3,4,5,6,7],temp=[];
var vari=(a)=>{for(var i=0;i<a.length;i++)
if(a[i]%2!=0)
temp.push(a[i]);return temp}
console.log((vari(a)));

*********************************************************************************

(b) Convert all the strings to title caps in a string array
===========================================================
var arr=["apple","beetroot","carrot","drumstick","eggplant","fig"];
var tit=(arr)=>{for(var i=0;i<arr.length;i++)
console.log(arr[i][0].toUpperCase()+arr[i].substr(1))}
tit(arr);

*********************************************************************************

(c) Sum of all numbers in an arry
=================================
var s=0;
var sum=(arr)=>{for(var i=0;i<arr.length;i++)s=s+arr[i];
return s}
console.log("Sum of array is:",sum([1,2,3,4,5,6,7]));

*********************************************************************************

(d) Return all the prime numbers in an array:
=============================================
const newArray = [1, 3, 2, 5, 10];
const isPrime = num => {
  for (let i = 2; i < num; i++) {
    if (num % i === 0) return false;
  }
  return num !== 1;
};

const myPrimeArray = newArray.filter(isPrime);
console.log(myPrimeArray);

*********************************************************************************

(e) Return all the palindromes in an array
==========================================
var a=["geek","lol","mam"]
var palindrome=(a) => {
  var temp=[];
for(var i=0;i<a.length;i++)
{var rev=a[i].split("").reverse().join("");
if(a[i]===rev)
temp.push(a[i]); }
    return temp;}
 console.log(palindrome(a));
 
*********************************************************************************

































