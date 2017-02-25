
function sumAll(arr) {
  
var fullArr = [];
var result;
  
var max = arr.reduce(function(a, b){
  return Math.max(a, b);
});

var min = arr.reduce(function(a, b){
  return Math.min(a, b);
});

  for (var i = min; i < max + 1; i++) {
    fullArr.push(i);
}

  result = fullArr.reduce(function(a, b) {
    return a + b;
  });
  
  return result;
}

sumAll([1, 4]);
