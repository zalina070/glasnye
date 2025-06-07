# glasnye
function findVowels(str) {
  const vowels = ['а', 'е', 'и', 'о', 'у'];
  let count = 0;

  for (let i = 0; i < str.length; i++) {
    if (vowels.includes(str[i].toLowerCase())) {
      count++;
    }
  }

  return count;
}

// Примеры:
console.log(findVowels("hello")); // -> 2 (e, o)
console.log(findVowels("why"));   // -> 0
console.log(findVowels("Привет")); // -> 2 (и, е)
