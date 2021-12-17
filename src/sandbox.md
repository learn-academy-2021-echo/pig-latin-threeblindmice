let currentWord = "spa"
let vowelsArray = currentWord.split("").filter(vowel => {
    return vowel === "a" || vowel === "e" || vowel === "i" || vowel === "o" || vowel === "u"
  })
var firstVow = currentWord.indexOf(vowelsArray[0])

 console.log(firstVow)
// so words beginning with consonates need to be split where the cons. and vowels meet. 
//add cons. to the end of word and add "ay"
console.log(currentWord.slice(firstVow))
  console.log(currentWord.slice(firstVow) + currentWord.slice(0,firstVow) + "ay")


  if (currentWord.slice(0,2) === "qu"){
    console.log(currentWord.slice(2) + currentWord.slice(0,2) + "ay")
} else if(currentWord.slice(1,3) === "qu"){
    console.log(currentWord.slice(3) + currentWord.slice(0,3) + "ay")
    
}else { 
        let firstCon = currentWord.slice(0,firstVow)
        let firstP = currentWord.slice(firstVow)
        console.log(firstP + firstCon + "ay")
    }    
