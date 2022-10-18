# Google-Colab-Tips
1.如何避免斷線? </br>
按下f12，並在console中輸入以下</br>
'''
function ClickConnect(){
console.log("Working");
document.querySelector("#top-toolbar > colab-connect-button").shadowRoot.querySelector("#connect").click();
}
setInterval(ClickConnect,60000)
'''
2.連線至google drive mount 
'''
from google.colab import drive
drive.mount('/content/drive')
'''
