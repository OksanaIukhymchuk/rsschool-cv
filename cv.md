# rsschool.cv
# [Rolling Scopes School](https://app.rs.school)
- - -
# Oksana Iukhymchuk
- - -
### **Contacts**

| **location** | *Kyiv, Ukraine* |
| ---------- | --------|
| **email** | *iukhymchuk.oksana@gmail.com* |
| **telegram** | *@oksanaiu* |


- - - 
### **Information**
My goal is to learn frontend and have the skills to create fun interactive sites, especially for educational purposes. I am passionate about growing professionally and learning from the people who already program in JavaScript. This is the reason I became the part of RS School JS Course. 
- - -
### **Skills** 
I started learning to code a year and a half ago when we all stayed home for quarantine. I have some basic knowledge in html, css, and js. I started to apply my knowledge creating the site: [IlearnRussian.net](https://www.ilearnrussian.net). It has examples of the code I wrote on my own, the code I adapted from workshops I took, the code modified by a mentor, and the free code I found on the internet and changed a little. These are my first efforts so do not judge me harshly.  
- - -
### **Work Experience**
I have not worked as programmer yet, except the site I have been creating: [ilearnRussian](https:www.ilearnrussian.net). I have been teaching Russian for foreigners and history of Ukraine for foreigners. 
- - -
### **English Level** 
C1, I majored in translating and teaching English. I have over 20 years of experience in communicating with native speakers and teaching in English.
- - -
### **Education** 
I have taken several courses on Udemy, watched and practiced a lot of workshops on youtube. My favorite teachers are:
* John Smilga (htmls&css) and 
* Dmitri Trepachov (Дмитрий Трепачёв, js). 


#### I took the following courses:
* [x] Udemy HTML&CSS Course - John Smilga;
* [x] Udemy Javascript Course - Jonas Schmedtmann;
* [x] HTML, CSS, JS Tutorials on the [w3schools](https://www.w3schools.com);
* [ ] [Dmitri Trepachov JS course](http://code.mu/ru/javascript/book/prime/) (in progress);
* [ ] [RS School Course "JS/FE. Stage 0"](https://app.rs.school/) (in progress);
* [ ] [Ilya Kantor JavaScript Book](https://learn.javascript.ru/) (in progress);

- - -
### **Code Example**
*I have written the code for this game fully by myself. A player needs to combine syllables to make words seen in the pictures. If the word is correct, they can see a picture next to it and a checkmark. But if the word is incorrect, it is marked wrong. They can keep working and checking their work until they make all the words.*
#### **It can be played here: [Match Syllables Game](https://ilearnrussian.net/alphabet/drag-drop/drag-drop-syllables_al1.html)**
![Match Syllables Game](match-syllables-game.png)
#### Part 1
```
let wordBankEasy = [    
    ['ко-ко-ко́', 'cluck-cluck', `<img class="picture" src="../alphabet_images/alphabet1/chicken_apng.png">`, '../alphabet_images/alphabet1/chicken_apng.png'],
    ['ма́ма', 'mom', '<img class="picture" src="../alphabet_images/alphabet1/mom_apng.png">', '../alphabet_images/alphabet1/mom_apng.png'],
    ['кот', 'cat', `<img class="picture" src="../alphabet_images/alphabet1/cat_apng.png">`, '../alphabet_images/alphabet1/cat_apng.png'],
    ['а́том', 'atom', `<img class="picture" src="../alphabet_images/alphabet1/atom_apng.png">`, '../alphabet_images/alphabet1/atom_apng.png'],
    ['кака́о', 'hot chocolate', `<img class="picture" src="../alphabet_images/alphabet1/hot-chocolate.png">`, '../alphabet_images/alphabet1/hot-chocolate.png'],
    ['мака́ка', 'macaque', `<img class="picture" src="../alphabet_images/alphabet1/macaque.png">`, '../alphabet_images/alphabet1/macaque.png'],
    ['та́ко', 'taco', `<img class="picture" src="../alphabet_images/alphabet1/taco.png">`, '../alphabet_images/alphabet1/taco.png'],
    ['ко́ма', 'coma', `<img class="picture" src="../alphabet_images/alphabet1/coma.png">`, '../alphabet_images/alphabet1/coma.png'],
    ['мак', 'Mac', `<img class="picture" src="../alphabet_images/alphabet1/mac.png">`, '../alphabet_images/alphabet1/mac.png'],
    ['Том', 'Tom', `<img class="picture" src="../alphabet_images/alphabet1/tom.png">`, '../alphabet_images/alphabet1/tom.png'],
    ['То́ма', 'Toma', `<img class="picture" src="../alphabet_images/alphabet1/toma.png">`, '../alphabet_images/alphabet1/toma.png'],
    ['мо́кко', 'espresso w/ hot milk and chocolate', `<img class="picture" src="../alphabet_images/alphabet1/coffee-mocca.png">`, '../alphabet_images/alphabet1/coffee-mocca.png'],
];

let wordBankHard = [
    ['мат', 'checkmate', `<img class="picture" src="../alphabet_images/alphabet1/checkmate.png">`, '../alphabet_images/alphabet1/checkmate.png'],        
    ['мат', 'mat', `<img class="picture" src="../alphabet_images/alphabet1/mat.png">`, '../alphabet_images/alphabet1/mat.png'],
    ['том', 'volume', `<img class="picture" src="../alphabet_images/alphabet1/volume-marx.png">`, '../alphabet_images/alphabet1/volume-marx.png'],
    ['ток', 'electrical current', `<img class="picture" src="../alphabet_images/alphabet1/electrical-current_apng.png">`, '../alphabet_images/alphabet1/electrical-current_apng.png'],
    ['мак', 'poppy flower', `<img class="picture" src="../alphabet_images/alphabet1/poppies.png">`, '../alphabet_images/alphabet1/poppies.png'],
    ['там', 'there', `<img class="picture" src="../alphabet_images/alphabet1/there.png">`, '../alphabet_images/alphabet1/there.png'],
    ['кто', 'who', `<img class="picture" src="../alphabet_images/alphabet1/who.png">`, '../alphabet_images/alphabet1/who.png'],
    ['ка́ка', 'poo', `<img class="picture" src="../alphabet_images/alphabet1/kaka.png">`, '../alphabet_images/alphabet1/kaka.png'],
    ['мо́ка', 'geiser coffee maker', `<img class="picture" src="../alphabet_images/alphabet1/moka.png">`, '../alphabet_images/alphabet1/moka.png'],
];
    
let wordBankPhrases = [
    ['кака́о кота́м', 'hot chocolate to the cats', `<img class="picture" src="../alphabet_images/alphabet1/chocholate-to-cats_apng.png">`, '../alphabet_images/alphabet1/chocolate-to-cats_apng.png'],
    ['кот Том', 'cat Tom', `<img class="picture" src="../alphabet_images/alphabet1/catTom.png">`, '../alphabet_images/alphabet1/catTom.png'],
    ['мак ма́мам', 'poppies to moms', `<img class="picture" src="../alphabet_images/alphabet1/poppies-to-moms.png">`, '../alphabet_images/alphabet1/poppies-to-moms.png'],
    ['та́ко мака́кам', 'taco for macaques', `<img class="picture" src="../alphabet_images/alphabet1/taco-to-macaques.png">`, '../alphabet_images/alphabet1/taco-to-macaques.png'],
    ['тот кот', 'that cat', `<img class="picture" src="../alphabet_images/alphabet1/that-cat.png">`, '../alphabet_images/alphabet1/that-cat.png'],
    ['тот мат', 'that mat', `<img class="picture" src="../alphabet_images/alphabet1/that-mat.png">`, '../alphabet_images/alphabet1/that-mat.png'],
    ['тот мак', 'that poppy', `<img class="picture" src="../alphabet_images/alphabet1/that-poppy.png">`, '../alphabet_images/alphabet1/that-poppy.png'],
    ['та ма́ма', 'that mom', `<img class="picture" src="../alphabet_images/alphabet1/that-mom.png">`, '../alphabet_images/alphabet1/that-mom.png'],
    ['та мака́ка', 'that macaque', `<img class="picture" src="../alphabet_images/alphabet1/that-macaque.png">`, '../alphabet_images/alphabet1/that-macaque.png'],
    ['то кака́о', 'that cocoa', `<img class="picture" src="../alphabet_images/alphabet1/that-hot-chocolate.png">`, '../alphabet_images/alphabet1/that-hot-chocolate.png'],
    ['то та́ко', 'that taco', `<img class="picture" src="../alphabet_images/alphabet1/that-taco.png">`, '../alphabet_images/alphabet1/that-taco.png'],
];
    

let wordBankSentences = [
    ['Кто там?', 'Who is there?', `<img class="picture" src="../alphabet_images/alphabet1/who-there.png">`, '../alphabet_images/alphabet1/who-there.png'],
    ['Там кот Том.', 'There is cat Tom there.', `<img class="picture" src="../alphabet_images/alphabet1/cat-tom-there.png">`, '../alphabet_images/alphabet1/cat-tom-there.png'],
    ['Там кака́о, а там та́ко.', 'There is hot chocolate there, and there\'s taco there.', `<img class="picture" src="../alphabet_images/alphabet1/hot-chocolate-taco-there.png">`, '../alphabet_images/alphabet1/hot-chocolate-taco-there.png'],
    ['Там ма́ма, а там То́ма.', 'There is mom, and there is Toma.', `<img class="picture" src="../alphabet_images/alphabet1/mom-toma-there.png">`, '../alphabet_images/alphabet1/mom-toma-there.png'],
    [`Там кот, а там Том. А там кот Том.`, 'There is the cat, and there is Tom. And there is cat Tom.', `<img class="picture" src="../alphabet_images/alphabet1/cat-tom-cattom-there.png">`, '../alphabet_images/alphabet1/cat-tom-cattom-there.png'],
    ['Там та мака́ка, а там - та.', 'There is that macaque there and there\'s that one. ', `<img class="picture" src="../alphabet_images/alphabet1/that-macaque-2.png">`, '../alphabet_images/alphabet1/that-macaque-2.png'],
    ['То та́ко там, а то - там.', 'That taco is there and that one is there.', `<img class="picture" src="../alphabet_images/alphabet1/that-taco-2.png">`, '../alphabet_images/alphabet1/that-taco-2.png'],
    ['Тот кот там, а тот - там.', 'That cat is there and that one is there.', `<img class="picture" src="../alphabet_images/alphabet1/that-cat-2.png">`, '../alphabet_images/alphabet1/that-cat-2.png'],
    ['Тот мак там, а тот - там.', 'That poppy is there and that one is there.', `<img class="picture" src="../alphabet_images/alphabet1/that-poppy-2.png">`, '../alphabet_images/alphabet1/that-poppy-2.png'],
];



let makeWordsSyllables = [
        ['ко-ко-ко́', 'cluck-cluck', `<img class="picture" src="../alphabet_images/alphabet1/chicken_apng.png">`, '../alphabet_images/alphabet1/chicken_apng.png'],
        ['ма́ма', 'mom', '<img class="picture" src="../alphabet_images/alphabet1/mom_apng.png">', '../alphabet_images/alphabet1/mom_apng.png'],
        ['а́том', 'atom', `<img class="picture" src="../alphabet_images/alphabet1/atom_apng.png">`, '../alphabet_images/alphabet1/atom_apng.png'],
        ['кака́о', 'hot chocolate', `<img class="picture" src="../alphabet_images/alphabet1/hot-chocolate.png">`, '../alphabet_images/alphabet1/hot-chocolate.png'],
        ['мака́ка', 'macaque', `<img class="picture" src="../alphabet_images/alphabet1/macaque.png">`, '../alphabet_images/alphabet1/macaque.png'],
        ['Том', 'Tom', `<img class="picture" src="../alphabet_images/alphabet1/tom.png">`, '../alphabet_images/alphabet1/tom.png'],
        ['та́ко', 'taco', `<img class="picture" src="../alphabet_images/alphabet1/taco.png">`, '../alphabet_images/alphabet1/taco.png'],
        ['ко́ма', 'coma', `<img class="picture" src="../alphabet_images/alphabet1/coma.png">`, '../alphabet_images/alphabet1/coma.png'],
        ['То́ма', 'Toma', `<img class="picture" src="../alphabet_images/alphabet1/toma.png">`, '../alphabet_images/alphabet1/toma.png'],
        ['мо́кко', 'espresso w/ hot milk and chocolate', `<img class="picture" src="../alphabet_images/alphabet1/coffee-mocca.png">`, '../alphabet_images/alphabet1/coffee-mocca.png'],
        ['ка́ка', 'poo', `<img class="picture" src="../alphabet_images/alphabet1/kaka.png">`, '../alphabet_images/alphabet1/kaka.png'],
        ['мо́ка', 'geiser coffee maker', `<img class="picture" src="../alphabet_images/alphabet1/moka.png">`, '../alphabet_images/alphabet1/moka.png'],
];


let letterSyllableBank = ['А', 'О', 'М', 'Т', 'К', 'ма', 'мо', 'ам', 'ом', 'ка', 'ко', 'ак', 'ок',  'та', 'то', 'ат', 'от' ]
let wordBankEasyHard = wordBankEasy.concat(wordBankHard);
let wordBankHardPhrases = wordBankHard.concat(wordBankPhrases);
let flashcardsBank = [
    ['тот', '"that" for nouns ending in a consonant', '', ''],
    ['та', '"that" for nouns ending in "A"', '', ''],
    ['то', '"that" for nouns ending in "O"', '', ''],
    ['а', 'but | and', '', ''],
    ['как', 'How?', '', ''],
    ['так', 'like this', '', ''],
]
flashcardsBank = flashcardsBank.concat(wordBankEasyHard);
```
#### Part 2
```
 <script>
        let syllables = [];
        let syllables1 = ['ко', 'ко', 'ко', 'ма', 'ма', 'а', 'том', 'ка', 'ка', 'о', 'ма', 'ка', 'ка', 'том'];
        let syllables2 = ['та', 'ко', 'ко', 'ма', 'то', 'ма', 'мок', 'ко', 'ка', 'ка', 'мо', 'ка'];  
        let pictures = [];
        for(let i = 0; i <makeWordsSyllables.length; i++) {
            pictures.push(makeWordsSyllables[i][2]);
        }

        let randomNumber = Math.ceil(Math.random() *2);
        document.querySelector('.set-number').innerHTML = `${randomNumber} / 2`;
        console.log(randomNumber)
        syllables = (randomNumber === 1) ? syllables1 : syllables2;
        syllables = syllables.sort(()=> Math.random() - 0.5);    


        let imagesDiv = document.querySelector('.images');
        imagesDiv.innerHTML = (randomNumber ===1) ? pictures.slice(0, 6).join('') : pictures.slice(6).join('');
    </script>
```
#### Part 3
```
let words = [];
        let images = [];

        let parentsContainer = document.querySelector('.parents-container');
        for(let i = 0; i<6; i++){
            let parentWrapper = document.createElement('div');
            parentWrapper.classList.add('parent-wrapper');
            parentsContainer.appendChild(parentWrapper);
            let parent = document.createElement('div');
            parent.classList.add('parent');
            let result = document.createElement('div');
            result.classList.add('result');
            parentWrapper.appendChild(parent);
            parentWrapper.appendChild(result);
        }


        let panel = document.getElementById('panel');
        for(let i = 0; i < syllables.length; i++){
            let elemWrapper = document.createElement('div');
            elemWrapper.classList.add('elem-wrapper');
            panel.appendChild(elemWrapper);
            let elemDiv = document.createElement('div');
            elemDiv.classList.add('elem');
            elemDiv.setAttribute('draggable', 'true');
            let elemDivText = document.createElement('div');
            elemDivText.classList.add('elem-text');
            elemDiv.appendChild(elemDivText);
            elemDivText.textContent = `${syllables[i]}`;
            elemWrapper.appendChild(elemDiv);
        };
    

        for(let i = 0; i <flashcardsBank.length; i++) {
            words.push(flashcardsBank[i][0].replace(/[-Ì]/g, '').toLowerCase());
            images.push(flashcardsBank[i][3]);
        }


       let elems = document.querySelectorAll('.elem');
       let parents = document.querySelectorAll('.parent');
       let results = document.querySelectorAll('.result');
       let score = 0;
        elems.forEach(function(elem) {
            elem.addEventListener('dragstart', function(event) {
                current = this;
            })
        });

        parents.forEach(function(parentElem) {
            parentElem.addEventListener('dragover', function(event) {
                event.preventDefault();
            })
        });

        parents.forEach(function(parentElem) {
            parentElem.addEventListener('drop', function(event) {
                this.appendChild(current);
        })
        });

        panel.addEventListener('dragover', function(event) {
            event.preventDefault();
        });

        panel.addEventListener('drop', function(event) {
            this.appendChild(current);
        });


        document.querySelector('.btn-check').addEventListener('click', checkResults);
        document.querySelector('.btn-again').addEventListener('click', init);

        function init() {
            window.location.reload();
        }
        function checkResults() {
            score = 0;
            parents.forEach(function(parent){
                let textContent = '';
                let elems = Array.from(parent.querySelectorAll('.elem'));
                elems.forEach(function(elem){
                    textContent += elem.textContent;
                })
                // score = 0;
                if(textContent ==='') return;
                else if(words.includes(textContent)) {
                    parent.parentElement .querySelector('.result').innerHTML = "âœ”ï¸ Good job!";
                    // score = score + 1 - words[textContent]
                    console.log(words.indexOf(textContent));
                    console.log(textContent);
                    score++;
                    document.querySelector('.score-paragraph').innerHTML = `Your score is <span class="emphasize">${score}</span> words out of 6.`;
                    parent.style.backgroundImage = `url('${images[words.indexOf(textContent)]}')`;
                    parent.style.backgroundPosition = 'right';
                    parent.style.backgroundSize = 'contain';
                    parent.style.backgroundRepeat = 'no-repeat';
                }
                else if(!words.includes(textContent)) {
                    parent.parentElement.querySelector('.result').innerHTML = "âŒ Think again!";
                    parent.style.backgroundImage = '';
                }
            });   
        };
```

