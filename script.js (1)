window.addEventListener("load", () => {

    setTimeout(() => {
        document.getElementById("loader").style.display = "none";
    }, 2500);

});

const music = document.getElementById("bgMusic");
const startBtn = document.getElementById("startBtn");

startBtn.addEventListener("click", () => {

    music.play();
heartBurst();
    startBtn.innerHTML = "❤️ I Love You ❤️";

    startBtn.style.transform = "scale(1.1)";

});

for (let i = 0; i < 40; i++) {

    let heart = document.createElement("div");

    heart.innerHTML = "❤";

    heart.style.position = "fixed";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.top = Math.random() * 100 + "vh";
    heart.style.fontSize = (10 + Math.random() * 25) + "px";
    heart.style.opacity = 0.15;
    heart.style.pointerEvents = "none";
    heart.style.animation = `float ${5 + Math.random() * 8}s linear infinite`;

    document.body.appendChild(heart);

}
const startDate = new Date("2026-03-08T00:00:00");

function updateTimer() {

    const now = new Date();

    const diff = now - startDate;

    const days = Math.floor(diff / (1000 * 60 * 60 * 24));

    const hours = Math.floor((diff / (1000 * 60 * 60)) % 24);

    const minutes = Math.floor((diff / (1000 * 60)) % 60);

    const seconds = Math.floor((diff / 1000) % 60);

    document.getElementById("days").innerHTML = days;
    document.getElementById("hours").innerHTML = hours;
    document.getElementById("minutes").innerHTML = minutes;
    document.getElementById("seconds").innerHTML = seconds;
}

updateTimer();
setInterval(updateTimer, 1000);
// Timeline animation
const cards = document.querySelectorAll(".card");

const observer = new IntersectionObserver((entries)=>{
    entries.forEach(entry=>{
        if(entry.isIntersecting){
            entry.target.style.opacity="1";
            entry.target.style.transform="translateY(0)";
        }
    });
});

cards.forEach(card=>{
    card.style.opacity="0";
    card.style.transform="translateY(50px)";
    card.style.transition="0.8s";
    observer.observe(card);
});
const galleryImages = document.querySelectorAll(".gallery img");
const lightbox = document.getElementById("lightbox");
const lightboxImg = document.getElementById("lightbox-img");
const closeBtn = document.querySelector(".close");

galleryImages.forEach(img => {
    img.addEventListener("click", () => {
        lightbox.style.display = "flex";
        lightboxImg.src = img.src;
    });
});'/'

closeBtn.addEventListener("click", () => {
    lightbox.style.display = "none";
});

lightbox.addEventListener("click", (e) => {
    if (e.target === lightbox) {
        lightbox.style.display = "none";
    }
});
const letterBtn = document.getElementById("letterBtn");
const letterBox = document.getElementById("letterBox");

letterBtn.addEventListener("click", () => {
    if (letterBox.style.display === "block") {
        letterBox.style.display = "none";
        letterBtn.innerText = "Read My Letter ❤️";
    } else {
        letterBox.style.display = "block";
        letterBtn.innerText = "Close Letter 💌";
    }
});

const musicBtn = document.getElementById("musicBtn");

musicBtn.addEventListener("click", () => {
    if (music.paused) {
        music.play();
        musicBtn.innerText = "⏸ Pause Music";
    } else {
        music.pause();
        musicBtn.innerText = "🎵 Play Music";
    }
});
function heartBurst() {

    for (let i = 0; i < 25; i++) {

        const heart = document.createElement("div");

        heart.innerHTML = "❤️";
        heart.className = "burst-heart";

        heart.style.left = (window.innerWidth / 2) + (Math.random() * 100 - 50) + "px";
        heart.style.top = (window.innerHeight / 2) + (Math.random() * 100 - 50) + "px";

        document.body.appendChild(heart);

        setTimeout(() => {
            heart.remove();
        }, 2000);

    }

}
function heartBurst() {

    for(let i = 0; i < 20; i++){

        const heart = document.createElement("div");

        heart.className = "burst-heart";
        heart.innerHTML = "❤️";

        heart.style.left = (window.innerWidth/2 + (Math.random()*200-100)) + "px";
        heart.style.top = (window.innerHeight/2 + (Math.random()*100-50)) + "px";

        document.body.appendChild(heart);

        setTimeout(()=>{
            heart.remove();
        },1800);

    }

}
const reveals = document.querySelectorAll(".reveal");

function revealOnScroll() {
    reveals.forEach(el => {
        const top = el.getBoundingClientRect().top;
        if (top < window.innerHeight - 100) {
            el.classList.add("active");
        }
    });
}

window.addEventListener("scroll", revealOnScroll);
revealOnScroll();
for(let i=0;i<60;i++){
    const sparkle=document.createElement("div");
    sparkle.className="sparkle";
    sparkle.style.left=Math.random()*100+"vw";
    sparkle.style.top=Math.random()*100+"vh";
    sparkle.style.animationDelay=Math.random()*3+"s";
    document.body.appendChild(sparkle);
}
function launchConfetti(){

    const colors = ["#ff4d88","#ff7fb2","#ffd166","#ffffff","#ffb3d9"];

    for(let i=0;i<120;i++){

        const confetti = document.createElement("div");
        confetti.className = "confetti";

        confetti.style.left = Math.random()*100 + "vw";
        confetti.style.background =
            colors[Math.floor(Math.random()*colors.length)];

        confetti.style.width = (6 + Math.random()*8) + "px";
        confetti.style.height = (6 + Math.random()*8) + "px";

        confetti.style.animationDuration =
            (2 + Math.random()*2) + "s";

        document.body.appendChild(confetti);

        setTimeout(()=>{
            confetti.remove();
        },4000);
    }
}

letterBtn.addEventListener("click", () => {
    launchConfetti();
});
const notes = [
    "❤️ You are my favourite notification.",
    "🌹 Every day with you is my favourite day.",
    "🥹 I still choose you. Every single time.",
    "💖 Forever Us. Forever Love.",
    "😘 I love you more than words can say."
];

const loveNote = document.createElement("div");
loveNote.className = "loveNote";
document.body.appendChild(loveNote);

function showLoveNote(){

    loveNote.innerText =
        notes[Math.floor(Math.random()*notes.length)];

    loveNote.style.opacity = "1";

    setTimeout(()=>{
        loveNote.style.opacity = "0";
    },4000);
}

setInterval(showLoveNote,30000);
let count = 0;
const reason = document.getElementById("reasonCount");

const counter = setInterval(() => {
    count += 7;
    reason.innerText = count;

    if (count >= 1000) {
        reason.innerText = "∞";
        clearInterval(counter);
    }
}, 15);
const endPopup = document.getElementById("endPopup");
const closePopup = document.getElementById("closePopup");

let popupShown = false;

window.addEventListener("scroll", () => {

    if (popupShown) return;

    const bottom =
        window.innerHeight + window.scrollY >=
        document.body.offsetHeight - 10;

    if (bottom) {
        popupShown = true;
        endPopup.classList.add("show");
    }

});

closePopup.addEventListener("click", () => {
    endPopup.classList.remove("show");
});
function createShootingStar() {

    const star = document.createElement("div");
    star.className = "shooting-star";

    star.style.left = Math.random() * window.innerWidth * 0.7 + "px";
    star.style.top = Math.random() * 200 + "px";

    document.body.appendChild(star);

    setTimeout(() => {
        star.remove();
    }, 1500);
}

setInterval(() => {
    createShootingStar();
}, 10000);

// First shooting star after 3 seconds
setTimeout(createShootingStar, 3000);
const openButtons = document.querySelectorAll(".openBtn");
const secretLetter = document.getElementById("secretLetter");

openButtons.forEach(button => {

    button.addEventListener("click", () => {

        secretLetter.style.display = "block";
        secretLetter.innerHTML = button.dataset.msg;

        secretLetter.scrollIntoView({
            behavior: "smooth",
            block: "center"
        });

    });

});
const memoryNotes = document.querySelectorAll(".memory-note");
const memoryPopup = document.getElementById("memoryPopup");

memoryNotes.forEach(note => {

    note.addEventListener("click", () => {

        memoryPopup.style.display = "block";
        memoryPopup.innerHTML = note.dataset.note;

        memoryPopup.scrollIntoView({
            behavior: "smooth",
            block: "center"
        });

    });

});
const lockBtn = document.getElementById("lockBtn");
const lock = document.querySelector(".lock");
const lockMessage = document.getElementById("lockMessage");

lockBtn.addEventListener("click", () => {

    lock.classList.add("open");

    lockMessage.style.display = "block";

    lockBtn.innerHTML = "❤️ Forever Locked ❤️";

    lockBtn.disabled = true;

});
/* ===== GRAND FINALE ===== */

const finalBtn = document.getElementById("finalBtn");
const finalMessage = document.getElementById("finalMessage");

if(finalBtn){

finalBtn.addEventListener("click",()=>{

    finalMessage.style.display="block";

    finalBtn.innerHTML="❤️ Forever Yours ❤️";
    finalBtn.disabled=true;

    finalMessage.animate([
        {opacity:0,transform:"translateY(40px)"},
        {opacity:1,transform:"translateY(0)"}
    ],{
        duration:1000,
        fill:"forwards"
    });

    // Heart Rain ❤️
    for(let i=0;i<80;i++){

        const heart=document.createElement("div");

        heart.innerHTML="❤️";

        heart.style.position="fixed";
        heart.style.left=Math.random()*100+"vw";
        heart.style.top="-30px";
        heart.style.fontSize=(18+Math.random()*28)+"px";
        heart.style.pointerEvents="none";
        heart.style.zIndex="99999";
        heart.style.transition="transform 5s linear, opacity 5s";

        document.body.appendChild(heart);

        setTimeout(()=>{
            heart.style.transform=`translateY(${window.innerHeight+150}px) rotate(${Math.random()*720}deg)`;
            heart.style.opacity="0";
        },50);

        setTimeout(()=>{
            heart.remove();
        },5200);
    }

    // Screen Glow ✨
    document.body.animate([
        {filter:"brightness(1)"},
        {filter:"brightness(1.35)"},
        {filter:"brightness(1)"}
    ],{
        duration:1800
    });

});
}