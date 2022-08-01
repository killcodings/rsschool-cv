![logo](https://sun9-52.userapi.com/impg/5qX6wdUO_BrFyNYIBCXVH2OyhPccwVhaUbcXow/t363U7EShpw.jpg?size=64x64&quality=96&proxy=1&sign=eac4cf2bab7bb7976a0ff39ddef3aab6&type=album "@killcodings")

# Kiryl Yakauchyk - junior front end developer

---

### Adress - Minsk, RB

### Email - <kontaktid@ya.ru>

### Github - <https://github.com/killcodings>

### Telegram - <https://t.me/killcodings>

---

## About me

I am a freelancer with little experience in web site development on WordPress. To date, I have created several websites with individual design. My hobbies are visiting thematic channels on the theme of programming, I am also interested in Game dev.

---

## Hard skills

- JavaScript
- HTML5
- CSS3
- FlexBox
- HTTP
- WordPress

---

## Sample Code:

    let arrayImg = document.querySelectorAll(".wrapper-img");
    let length = arrayImg.length;

    let menuUl = document.querySelector(".menu");
    let arrayText = document.querySelectorAll(".text");
    let arrayMenuLi = document.querySelectorAll(".menu-item");
    let lengthMenuLi = arrayMenuLi.length;
    let tabName;

    let wrapImg = document.querySelector(".content_img");
    let popup = document.querySelector(".popup");
    let popupImg = document.querySelector(".popup .wrapper-img img");

    let button = document.querySelector('.button');




    function changeImage() {
    	for (let i = 0; i < length; i++) {
    		if(i !== length - 1 && arrayImg[i].classList.contains("active_image")) {
    			arrayImg[i].classList.remove("active_image");
    			arrayImg[i + 1].classList.add("active_image");
    			return;
    		} else if (i == length - 1 && arrayImg[i].classList.contains("active_image")) {
    			arrayImg[i].classList.remove("active_image");
    			arrayImg[0].classList.add("active_image");
    			return;
    		}
    	}
    }

    // setInterval(changeImage, 5000);


    // Tab

    function removeActiveclass() {
    	for (let i = 0; i < lengthMenuLi; i++) {
    		if (arrayMenuLi[i].classList.contains('menu_active')) {
    			arrayMenuLi[i].classList.remove("menu_active");
    		}
    	}
    }

    function removeActiveDiv() {
    	for (let i = 0; i < lengthMenuLi; i++) {
    		if (arrayText[i].classList.contains('active')) {
    			arrayText[i].classList.remove('active');
    		}
    	}
    }

    menuUl.addEventListener('click', function(e){
    	console.log(e);
        if(e.target.parentElement.classList.contains('menu-item') && !e.target.parentElement.classList.contains('menu_active')) {
            removeActiveclass();
            removeActiveDiv();
            e.target.parentElement.classList.add('menu_active');

            let id = e.target.parentElement.getAttribute('id');
            arrayText[id].classList.add('active')
        }
    });

    // PopupImg


    wrapImg.addEventListener('click', function(e) {
    	if(e.target.parentElement.classList.contains('wrapper-img')){
    		let src = e.target.getAttribute('src');
    		popupImg.setAttribute('src', src);
    		popup.classList.add('popup__active');
    	}
    });

    popup.addEventListener('click', function(e) {
    	if (e.target.classList.contains('close') || e.target.parentElement.classList.contains('close')) {
            popup.classList.remove('popup__active');
    	}
    });



    // scrollIntoView

    function handleButtonClick() {
       wrapImg.scrollIntoView({block: "center", behavior: "smooth"});
    }

    button.addEventListener('click', handleButtonClick);

---

## Projects

- <https://ardonit.ru/>
- <https://dk-mebel.com/>
- <http://iso.promhim-group.com/>
- <http://sub-eurogroup.topevent.by/>

---

## Education

2011-2016
: **Belarusian State University Institute of Business and Technology Management**

2005-2009
: **Minsk State Engineering College**

---

## Languages

English: Elementary
