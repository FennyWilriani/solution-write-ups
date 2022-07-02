# 7 kyu

# [Consecutive Vowels in a String](https://www.codewars.com/kata/62a933d6d6deb7001093de16)

This function is to find out how many ordered and consecutive vowels there are
in the given string beginning from "a"

## Syntax

> characters (string) --> result (number)

### Parameters

**Word**: `String`

- String of lower-case characters

### Return Value: `Number`

- An integer with the length of the consecutive vowels found

## Test Cases

Test case from Codewars:

```js
const chai = require('chai');
const assert = chai.assert;

describe('Simple Tests', function () {
  it('Very short string', function () {
    const s = 'akfheujfkgiaaaofmmfkdfuaiiie';
    assert.equal(getTheVowels(s), 7, s);
  });

  it('No "a" in string', function () {
    const s = 'eiknfhjrytueiouesxdczbeuiuoimnmfhfiuou';
    assert.equal(getTheVowels(s), 0, s);
  });

  it('Full cycle test', function () {
    let s =
      'desrehakkjfuteknvfiyrtfbehjdjrobchrunbcbbhdhehbvudjsnanbakkjndhfjenfndinmfnbfondndendnfudnfnanndhdemdmcnfdemnfjimdfofnmfnfjanmdnhdua';
    assert.equal(getTheVowels(s), 16, s);
    s =
      'sudnfhrakekdhhfkakjdjdhvneidkvnudntomcnnamjemdmfudkfhjamvcjedkfdnridnmnbvfhbdjdidncbvchencchdjdodncvchfndnrnencncnffduncbhjdfja';
    assert.equal(getTheVowels(s), 11, s);
    s =
      'jurjfdleiifjriisiouajjfyhekkfjvnnmsuimsnvyuhvcodnmfnsumvbjshhsadkvhfeixoua';
    assert.equal(getTheVowels(s), 11, s);
  });
});
```

## Examples

This function is using `for` loop, and `if/else` statement to iterate the index
of the string & vowels.

```js
// use case
function getTheVowels(word) {
  let vowels = 'aeiou',
    vowelsIndex = 0,
    result = 0;
  for (let index = 0; index < word.length; index++) {
    if (word[index] == vowels[vowelsIndex]) {
      result++;
      if (vowelsIndex == 4) {
        vowelsIndex = 0;
      } else {
        vowelsIndex++;
      }
    }
  }
  return result;
}

let example = getTheVowels('agrtertyfikfmroyrntbvsukldkfa');
console.log(example); // result 6
```

---

---

> user's solution to this challenge

## [cave.on](https://www.codewars.com/users/cave.on)

Using split() & reduce() methods

```js
const getTheVowels = (word, vowels = 'aeiou') =>
  word
    .split('')
    .reduce(
      (count, char) => count + (char === vowels[count % vowels.length]),
      0,
    );

const example = getTheVowels('agrtertyfikfmroyrntbvsukldkfa');
console.log(example); // result 6
```

## [NunoOliveira](https://www.codewars.com/users/NunoOliveira)

Using reduce() methods

```js
const getTheVowels = (string, vowels = 'aeiou') =>
  Array.from(string).reduce(
    (length, character) =>
      length + (character === vowels.charAt(length % vowels.length)),
    0,
  );

const example = getTheVowels('agrtertyfikfmroyrntbvsukldkfa');
console.log(example); // result 6
```

## Retrospective

<!--
  write any notes to help you review this exercise later, and to help others' study it.

  this might include:

  - good ideas to use later in your own code
  - less good ideas to avoid in your own code
  - new vocabulary you learned
  - the most important thing(s) you learned
  - something that you still don't understand but want to keep studying
  - something that surprised you
  - tricks you will want to remember and use later
-->

### Continue Doing

### Start Doing

### Stop Doing
