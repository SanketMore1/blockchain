# blockchain
all work relates to blockchain on remix ide

#1
pragma solidity ^0.8.17;
contract HelloWorld {
function print( ) public pure returns (string memory) {
return "Hello World !";
}
}


#2
pragma solidity ^0.8.17;
contract Storage {
uint256 n;
function store( ) public {
n = 5;
}
function get( ) public view returns (uint256) {
return n;
}
}
 #3
 pragma solidity ^0.8.17;
contract Greeter {
string private _greeting;
function greet (string memory message) public {
_greeting = message;
}
function getGreeting( ) public view returns (string memory) {
return _greeting;
}

}

#4
pragma solidity ^0.8.17;
contract Calculator {
function add(int a, int b) public pure returns (int){
return (a+b);
}
function sub(int a, int b) public pure returns (int){
return (a-b);
}
function mul(int a, int b) public pure returns (int){
return (a*b);
}
function div(int a, int b) public pure returns (int){
return (a/b);
}
}

#5
pragma solidity ^0.8.17;
contract EvenOdd {
function check(int num) public pure returns (string memory){
if(num % 2 == 0)
return "EVEN";
return "ODD";
}

}


#6
pragma solidity ^0.8.17;
contract ThreeAndSeven {
function check(int num) public pure returns (bool){
if((num % 3 == 0 || num % 7 == 0) && num > 10)
return true;
return false;
}
}



#7


pragma solidity ^0.8.17;
contract PrimeNumber {
function ifPrime(int num) public pure returns (bool) {
if (num == 1) return false;
for(int i = 2; i < num; i++){
if(num % i == 0)
return false;
}
return true;
}
}

