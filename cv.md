# Oleksandr Gubskyy
### Contact info:
#### Email: aleks.gubskyy@gmail.com
#### Telephone: +48537628155
#### Website: [Agubskyy.com](http://agubskyy.com)

### Summary
Front-end developer with a passion for great projets and unique solutions. I like to constantly improve my knowledge and skills and create something truly amazing. Currently I am gaining as much experience as I can through variety of different projects. I do mostly my own projects and had some amazing time working on behalf of different companies to 

### Skills
* HTML5 and CSS3
* Vanilla JavaScript (ES6)
* React.js
* REST API
* Node.js
* Unit Testing:
 * Jest
 
### Code Samples:

**Validating brackets task with futher testing**

```javascript
module.exports = function check(str, bracketsConfig) {
    let brArray = str.split("")
    let stack = []

    let bracketsOptions = bracketsConfig.map(el => el.join("")).join("")
    if (str.length % 2 !== 0) { return false }
    brArray.forEach(el => {
        for (let n = 0; n < bracketsOptions.length; n += 2) {

            let m = n + 1

            if (el == bracketsOptions[m]
                && bracketsOptions[n] == bracketsOptions[m]
                && bracketsOptions[n] == stack[stack.length - 1]) {
                stack.pop()
            } else if (el == bracketsOptions[n]
                && bracketsOptions[n] == bracketsOptions[m]
                && bracketsOptions[n] !== stack[stack.length - 1]) {
                stack.push(el)
            }

            if (el == bracketsOptions[n] && bracketsOptions[n] !== bracketsOptions[m]) {
                stack.push(el)
            } else if (el == bracketsOptions[m] && bracketsOptions[n] !== bracketsOptions[m]) {
                if (bracketsOptions[n] == stack[stack.length - 1]) {
                    stack.pop()
                } else {
                    return false
                }
            }
        }
    })

    return (stack.length == 0)
}
``` 

### Experience
**Freelance Web Dev from 2018, working on such projects: **

Project | Link | Codebase
------------ | ------------- |----------
Space Shooter Template | [Koji.com](https://withkoji.com/~FrostyDog/c094cf76-cd62-46c3-b9a4-84099d758b4a) | [Codebase on Koji.com](https://withkoji.com/~FrostyDog/c094cf76-cd62-46c3-b9a4-84099d758b4a)
PainWorkshop website (React.js) | [PainWorkshop.pl](http://painworkshop.pl/) | [Codebase](https://github.com/FrostyDog/Tattoo-Pain-Studio)

### Education

* **RS School - Frontend Mentorship Programm**
* **Javascript Udemy bootcamp**

### English
**English Level - C1 (Proficient)**
**IELTS English testing - 7,5 / 9**
**Studying in USA and Canada**



