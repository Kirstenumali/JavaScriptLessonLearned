# JavaScriptLessonLearned

A. Developers must include a comma when they add another function inside the script section in Vue.js.
``` bash
 showscriptcontrolls () {
      const scriptcontrollspannel = document.getElementById('scriptcontrolls') as HTMLHtmlElement
      scriptcontrollspannel!.style.display = 'block'
      setTimeout(() => {
        this.hidescriptcontrolls()
      }, 10000)
    },
```
B. Developers use the async keyword to write asynchronous code effectively.
``` bash
  async getPromptFromServer () {
      try {
        const response = await fetch('')
        const data = await response.json()
        this.promptdata = data['0']
      } catch (error) {
        console.log('error')
      }
    },
```
C. Developers can place logic statements outside the curly braces of try-catch, if-else, and while blocks.
``` bash
 abort () {
      const robot = window.api
      robot.dialogService.abortRR()
      robot.scriptsService.stopScript()
      if (this.audioPlayer) {
        this.audioPlayer.pause()
        this.audioPlayer.currentTime = 0
        this.onAudioEnded()
      }
      window.api.digService.externalPlayStop()
    },
```
D. Developers must add a space between the function keyword and the method name.
``` bash
 abort () {
      const robot = window.api
      robot.dialogService.abortRR()
      robot.scriptsService.stopScript()
      if (this.audioPlayer) {
        this.audioPlayer.pause()
        this.audioPlayer.currentTime = 0
        this.onAudioEnded()
      }
      window.api.dialogService.externalPlayStop()
    },
```
E. Developers must use lowerCamelCase when naming functions and variables.
``` bash
 handleCheckboxChange (event: Event) {
      const target = event.target as HTMLInputElement
      this.isChecked = target.checked
      if (this.isChecked) {
        console.log('true')
        this.scripttoggle = true
        if (this.audioPlayer) {
          this.audioPlayer.src = require('../')
          this.audioPlayer.play()
        }
      } else {
        console.log('false')
        this.scripttoggle = false
      }
    },
```
F. Developers must use parameters to make other functions accessible and reusable.
``` bash
 handleCheckboxChange (event: Event) {
      const target = event.target as HTMLInputElement
      this.isChecked = target.checked
      if (this.isChecked) {
        console.log('true')
        this.scripttoggle = true
        if (this.audioPlayer) {
          this.audioPlayer.src = require('../.mp3')
          this.audioPlayer.play()
        }
      } else {
        console.log('false')
        this.scripttoggle = false
      }
    },
```
G. Developers define a methods: {} block in the script section to organize and contain reusable methods.
``` bash
methods: {
    async getServerFromServer () {
      try {
        const response = await fetch('')
        const data = await response.json()
        this.promptdata = data['0']
      } catch (error) {
        console.log('error')
      }
    }}
```
