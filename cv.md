# **Misyukevich Darya**
## Contacts
E-mail: <missukevitch@gmail.com>  
Phone: [+375 (29) 573 10 79](tel:+375295731079)
## Summary
I want to became a good web developer. I hope that my work will bring me pleasure and good income. I am purposeful, hardworking and I have a great desire to learn and develop.
## Skills
* Figma, Photoshop, Illustrator
* HTML
* CSS
* JS
* C++  
## Code examples  
`````javascript    
const inputArray = () => {
	for(let i = 0; i < n; i++) {
		array[i] = parseFloat(prompt(`Введите ${i+1} элемент массива`));
		console.log(array[i]);
	}
}

const selectSort = () => {
	for (let i = 0; i < n - 1; i++)
	{
		let ind = i;
		let min = array[i];
		for (let j = i + 1; j < n; j++)
		{
			if (array[j] < min)
			{
				[ind, min] = [j, array[j]];
			}
		}
		if (ind != i)
		{
			[array[i],array[ind]] = [array[ind],array[i]];
		}
	}
};

const sumOfElements = () => {
	let sum = 0;
	for (let i = 0; i < n; i++) {
		sum += array[i];
	}
	return sum;
};

const minimum = () => {
	let min = array[0];
	for (let i = 0; i < n; i++){
		if (array[i] < min)
			min = array[i];
	}
	return min;
};

const maximum = () => {
	let max = array[0];
	for (let i = 0; i < n; i++){
		if (array[i] > max)
			max = array[i];
	}
	return max;
};

const n = prompt('Сколько элементов будет в массиве?');
console.log(n);
let array = [];
inputArray();
console.log('Исходный массив: ' + array);
selectSort();
console.log('Отсортированный массив: ' + array);
console.log('Сумма: ' + sumOfElements());
console.log('Минимальный элемент: ' + array[0]);
console.log('Максимальный элемент: ' + array[n - 1]);
`````