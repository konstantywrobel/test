# Test 

```

function test() {
	
	let total = 3;
	let correct = 0;
	let alertText;
	let i;
	
	let a1 = document.getElementById('q1').value;
	if(a1 == '1000') {
		correct++;
	}
	
	let a2 = document.getElementsByName('q2');
	for(i = 0; i < a2.length; i++) {
		if(a2[i].checked) {
			if(a2[i].value == 'true') {
				correct++;
				break;
			}
		}
	}
	
	let a3 = document.getElementsByName('q3');
	for(i = 0; i < a3.length; i++) {
		if(a3[i].checked) {
			if(a3[i].value == '2') {
				correct++;
				break;
			}
		}
	}
	
	if(correct == total) {
		alertText = "Congratulations! You have all the questions right!";
	}
	else {
		alertText = "You have " + correct + " out of " + total + " correct!";
	}
	alert(alertText);
}

```

## Example

[demo](http://konstantyw.pl/test)
