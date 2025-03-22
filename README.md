<!DOCTYPE html>
<html lang="en" >
<head>
    <meta charset="UTF-8">
    <title>Безопасный Интернет</title>
    <link rel="icon" type="icon" href="images\icon.svg">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="https://public.codepenassets.com/css/reset-2.0.min.css">
<style>
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@600&display=swap");
body {
  height: 300px;
  background-image: url(https://avatars.mds.yandex.net/i?id=940c9b9982d21d623ac97610bbbef469975d878f-4569079-images-thumbs&n=13);
  background-size: cover;
  background-position: 50% 50%;
  background-attachment: fixed;
  font-family: "Open Sans", sans-serif;
  padding-left: 115px;
}
.navbar {
  position: fixed;
  top: 1rem;
  left: 1rem;
  background: #ffffff4f;
  border-radius: 10px;
  padding: 1rem 0;
  box-shadow: 0 0 40px rgba(0, 0, 0, 0.03);
  height: calc(100vh - 4rem);
   border-bottom: 3px solid lime; 
}
.navbar__link {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 3.5rem;
  width: 5.5rem;
  color: #6a778e;
  transition: 250ms ease all;
}
.navbar__link span {
  position: absolute;
  left: 100%;
  transform: translate(-3rem);
  margin-left: 1rem;
  opacity: 0;
  pointer-events: none;
  color: #406ff3;
  background: #ffffff;
  padding: 0.75rem;
  transition: 250ms ease all;
  border-radius: 17.5px;
}
.navbar__link:hover {
  color: #fff;
}
.navbar:not(:hover) .navbar__link:focus span, .navbar__link:hover span {
  opacity: 1;
  transform: translate(0);
}
.navbar__menu {
  position: relative;
}
.navbar__item:last-child:before {
  content: "";
  position: absolute;
  opacity: 0;
  z-index: -1;
  top: 0;
  left: 1rem;
  width: 3.5rem;
  height: 3.5rem;
  background: #406ff3;
  border-radius: 17.5px;
  transition: 250ms cubic-bezier(1, 0.2, 0.1, 1.2) all;
}
.navbar__item:first-child:nth-last-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(1) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(1):last-child:hover:before, .navbar__item:first-child:nth-last-child(1) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(1):last-child:hover:before, .navbar__item:first-child:nth-last-child(1) ~ li:last-child:hover:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(2) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(2):last-child:hover:before, .navbar__item:first-child:nth-last-child(2) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(2):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(2) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(2):last-child:hover:before, .navbar__item:first-child:nth-last-child(2) ~ li:last-child:hover:before {
  top: 50%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(3):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(3) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(3):last-child:hover:before, .navbar__item:first-child:nth-last-child(3) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(3):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(3) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(3):nth-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(3) ~ li:nth-child(2):hover ~ li:last-child:before {
  top: 33.3333333333%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(3):last-child:hover:before, .navbar__item:first-child:nth-last-child(3) ~ li:last-child:hover:before {
  top: 66.6666666667%;
  animation: gooeyEffect-3 250ms 1;
}
@keyframes gooeyEffect-3 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(4):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(4) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(4):last-child:hover:before, .navbar__item:first-child:nth-last-child(4) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(4):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(4) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(4):nth-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(4) ~ li:nth-child(2):hover ~ li:last-child:before {
  top: 25%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(4):nth-child(3):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(4) ~ li:nth-child(3):hover ~ li:last-child:before {
  top: 50%;
  animation: gooeyEffect-3 250ms 1;
}
@keyframes gooeyEffect-3 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(4):last-child:hover:before, .navbar__item:first-child:nth-last-child(4) ~ li:last-child:hover:before {
  top: 75%;
  animation: gooeyEffect-4 250ms 1;
}
@keyframes gooeyEffect-4 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(5):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(5) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(5):last-child:hover:before, .navbar__item:first-child:nth-last-child(5) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(5):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(5) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(5):nth-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(5) ~ li:nth-child(2):hover ~ li:last-child:before {
  top: 20%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(5):nth-child(3):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(5) ~ li:nth-child(3):hover ~ li:last-child:before {
  top: 40%;
  animation: gooeyEffect-3 250ms 1;
}
@keyframes gooeyEffect-3 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(5):nth-child(4):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(5) ~ li:nth-child(4):hover ~ li:last-child:before {
  top: 60%;
  animation: gooeyEffect-4 250ms 1;
}
@keyframes gooeyEffect-4 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(5):last-child:hover:before, .navbar__item:first-child:nth-last-child(5) ~ li:last-child:hover:before {
  top: 80%;
  animation: gooeyEffect-5 250ms 1;
}
@keyframes gooeyEffect-5 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(6):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(6) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(6):last-child:hover:before, .navbar__item:first-child:nth-last-child(6) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(6):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(6) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(6):nth-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(6) ~ li:nth-child(2):hover ~ li:last-child:before {
  top: 16.6666666667%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(6):nth-child(3):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(6) ~ li:nth-child(3):hover ~ li:last-child:before {
  top: 33.3333333333%;
  animation: gooeyEffect-3 250ms 1;
}
@keyframes gooeyEffect-3 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(6):nth-child(4):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(6) ~ li:nth-child(4):hover ~ li:last-child:before {
  top: 50%;
  animation: gooeyEffect-4 250ms 1;
}
@keyframes gooeyEffect-4 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(6):nth-child(5):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(6) ~ li:nth-child(5):hover ~ li:last-child:before {
  top: 66.6666666667%;
  animation: gooeyEffect-5 250ms 1;
}
@keyframes gooeyEffect-5 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(6):last-child:hover:before, .navbar__item:first-child:nth-last-child(6) ~ li:last-child:hover:before {
  top: 83.3333333333%;
  animation: gooeyEffect-6 250ms 1;
}
@keyframes gooeyEffect-6 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(7):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(7) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(7):last-child:hover:before, .navbar__item:first-child:nth-last-child(7) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(7):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(7) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(7):nth-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(7) ~ li:nth-child(2):hover ~ li:last-child:before {
  top: 14.2857142857%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(7):nth-child(3):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(7) ~ li:nth-child(3):hover ~ li:last-child:before {
  top: 28.5714285714%;
  animation: gooeyEffect-3 250ms 1;
}
@keyframes gooeyEffect-3 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(7):nth-child(4):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(7) ~ li:nth-child(4):hover ~ li:last-child:before {
  top: 42.8571428571%;
  animation: gooeyEffect-4 250ms 1;
}
@keyframes gooeyEffect-4 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(7):nth-child(5):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(7) ~ li:nth-child(5):hover ~ li:last-child:before {
  top: 57.1428571429%;
  animation: gooeyEffect-5 250ms 1;
}
@keyframes gooeyEffect-5 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(7):nth-child(6):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(7) ~ li:nth-child(6):hover ~ li:last-child:before {
  top: 71.4285714286%;
  animation: gooeyEffect-6 250ms 1;
}
@keyframes gooeyEffect-6 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(7):last-child:hover:before, .navbar__item:first-child:nth-last-child(7) ~ li:last-child:hover:before {
  top: 85.7142857143%;
  animation: gooeyEffect-7 250ms 1;
}
@keyframes gooeyEffect-7 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(8):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(8) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(8):last-child:hover:before, .navbar__item:first-child:nth-last-child(8) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(8):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(8) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(8):nth-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(8) ~ li:nth-child(2):hover ~ li:last-child:before {
  top: 12.5%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(8):nth-child(3):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(8) ~ li:nth-child(3):hover ~ li:last-child:before {
  top: 25%;
  animation: gooeyEffect-3 250ms 1;
}
@keyframes gooeyEffect-3 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(8):nth-child(4):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(8) ~ li:nth-child(4):hover ~ li:last-child:before {
  top: 37.5%;
  animation: gooeyEffect-4 250ms 1;
}
@keyframes gooeyEffect-4 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(8):nth-child(5):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(8) ~ li:nth-child(5):hover ~ li:last-child:before {
  top: 50%;
  animation: gooeyEffect-5 250ms 1;
}
@keyframes gooeyEffect-5 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(8):nth-child(6):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(8) ~ li:nth-child(6):hover ~ li:last-child:before {
  top: 62.5%;
  animation: gooeyEffect-6 250ms 1;
}
@keyframes gooeyEffect-6 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(8):nth-child(7):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(8) ~ li:nth-child(7):hover ~ li:last-child:before {
  top: 75%;
  animation: gooeyEffect-7 250ms 1;
}
@keyframes gooeyEffect-7 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(8):last-child:hover:before, .navbar__item:first-child:nth-last-child(8) ~ li:last-child:hover:before {
  top: 87.5%;
  animation: gooeyEffect-8 250ms 1;
}
@keyframes gooeyEffect-8 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(9):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(9) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(9):last-child:hover:before, .navbar__item:first-child:nth-last-child(9) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(9):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(9) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(9):nth-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(9) ~ li:nth-child(2):hover ~ li:last-child:before {
  top: 11.1111111111%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(9):nth-child(3):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(9) ~ li:nth-child(3):hover ~ li:last-child:before {
  top: 22.2222222222%;
  animation: gooeyEffect-3 250ms 1;
}
@keyframes gooeyEffect-3 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(9):nth-child(4):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(9) ~ li:nth-child(4):hover ~ li:last-child:before {
  top: 33.3333333333%;
  animation: gooeyEffect-4 250ms 1;
}
@keyframes gooeyEffect-4 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(9):nth-child(5):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(9) ~ li:nth-child(5):hover ~ li:last-child:before {
  top: 44.4444444444%;
  animation: gooeyEffect-5 250ms 1;
}
@keyframes gooeyEffect-5 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(9):nth-child(6):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(9) ~ li:nth-child(6):hover ~ li:last-child:before {
  top: 55.5555555556%;
  animation: gooeyEffect-6 250ms 1;
}
@keyframes gooeyEffect-6 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(9):nth-child(7):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(9) ~ li:nth-child(7):hover ~ li:last-child:before {
  top: 66.6666666667%;
  animation: gooeyEffect-7 250ms 1;
}
@keyframes gooeyEffect-7 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(9):nth-child(8):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(9) ~ li:nth-child(8):hover ~ li:last-child:before {
  top: 77.7777777778%;
  animation: gooeyEffect-8 250ms 1;
}
@keyframes gooeyEffect-8 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(9):last-child:hover:before, .navbar__item:first-child:nth-last-child(9) ~ li:last-child:hover:before {
  top: 88.8888888889%;
  animation: gooeyEffect-9 250ms 1;
}
@keyframes gooeyEffect-9 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(10):last-child:hover:before, .navbar__item:first-child:nth-last-child(10) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(10):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):nth-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:nth-child(2):hover ~ li:last-child:before {
  top: 10%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):nth-child(3):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:nth-child(3):hover ~ li:last-child:before {
  top: 20%;
  animation: gooeyEffect-3 250ms 1;
}
@keyframes gooeyEffect-3 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):nth-child(4):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:nth-child(4):hover ~ li:last-child:before {
  top: 30%;
  animation: gooeyEffect-4 250ms 1;
}
@keyframes gooeyEffect-4 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):nth-child(5):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:nth-child(5):hover ~ li:last-child:before {
  top: 40%;
  animation: gooeyEffect-5 250ms 1;
}
@keyframes gooeyEffect-5 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):nth-child(6):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:nth-child(6):hover ~ li:last-child:before {
  top: 50%;
  animation: gooeyEffect-6 250ms 1;
}
@keyframes gooeyEffect-6 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):nth-child(7):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:nth-child(7):hover ~ li:last-child:before {
  top: 60%;
  animation: gooeyEffect-7 250ms 1;
}
@keyframes gooeyEffect-7 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):nth-child(8):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:nth-child(8):hover ~ li:last-child:before {
  top: 70%;
  animation: gooeyEffect-8 250ms 1;
}
@keyframes gooeyEffect-8 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):nth-child(9):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(10) ~ li:nth-child(9):hover ~ li:last-child:before {
  top: 80%;
  animation: gooeyEffect-9 250ms 1;
}
@keyframes gooeyEffect-9 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(10):last-child:hover:before, .navbar__item:first-child:nth-last-child(10) ~ li:last-child:hover:before {
  top: 90%;
  animation: gooeyEffect-10 250ms 1;
}
@keyframes gooeyEffect-10 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:hover ~ li:last-child:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(11):last-child:hover:before, .navbar__item:first-child:nth-last-child(11) ~ li:last-child:hover:before {
  opacity: 1;
}
.navbar__item:first-child:nth-last-child(11):nth-child(1):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(1):hover ~ li:last-child:before {
  top: 0%;
  animation: gooeyEffect-1 250ms 1;
}
@keyframes gooeyEffect-1 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):nth-child(2):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(2):hover ~ li:last-child:before {
  top: 9.0909090909%;
  animation: gooeyEffect-2 250ms 1;
}
@keyframes gooeyEffect-2 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):nth-child(3):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(3):hover ~ li:last-child:before {
  top: 18.1818181818%;
  animation: gooeyEffect-3 250ms 1;
}
@keyframes gooeyEffect-3 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):nth-child(4):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(4):hover ~ li:last-child:before {
  top: 27.2727272727%;
  animation: gooeyEffect-4 250ms 1;
}
@keyframes gooeyEffect-4 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):nth-child(5):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(5):hover ~ li:last-child:before {
  top: 36.3636363636%;
  animation: gooeyEffect-5 250ms 1;
}
@keyframes gooeyEffect-5 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):nth-child(6):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(6):hover ~ li:last-child:before {
  top: 45.4545454545%;
  animation: gooeyEffect-6 250ms 1;
}
@keyframes gooeyEffect-6 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):nth-child(7):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(7):hover ~ li:last-child:before {
  top: 54.5454545455%;
  animation: gooeyEffect-7 250ms 1;
}
@keyframes gooeyEffect-7 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):nth-child(8):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(8):hover ~ li:last-child:before {
  top: 63.6363636364%;
  animation: gooeyEffect-8 250ms 1;
}
@keyframes gooeyEffect-8 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):nth-child(9):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(9):hover ~ li:last-child:before {
  top: 72.7272727273%;
  animation: gooeyEffect-9 250ms 1;
}
@keyframes gooeyEffect-9 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):nth-child(10):hover ~ li:last-child:before, .navbar__item:first-child:nth-last-child(11) ~ li:nth-child(10):hover ~ li:last-child:before {
  top: 81.8181818182%;
  animation: gooeyEffect-10 250ms 1;
}
@keyframes gooeyEffect-10 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.navbar__item:first-child:nth-last-child(11):last-child:hover:before, .navbar__item:first-child:nth-last-child(11) ~ li:last-child:hover:before {
  top: 90.9090909091%;
  animation: gooeyEffect-11 250ms 1;
}
@keyframes gooeyEffect-11 {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(0.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
}
.myicon {
    stroke: #ff0000; /* Цвет иконки */
}
.h3 {
  font-size: 18px; /*Из за внешних стилей придется создавать размеры текста в ручную */
}
.h2 {
  font-size: 24px;
}
.h1 {
  font-size: 30px;
}
.end {
  margin: 10px;
  padding: 5px;
}
</style>
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script><!--Библиотека-->
</head>
<body translate="no">
    <center> <br>
    <img src="images\image (2).png"alt="Безопасный Интернет">
    </center>

  <nav class="navbar"> <!--Боковое меню--> 
  <ul class="navbar__menu">
    <li class="navbar__item"> 
      <a href="Кража персональных данных..html" class="navbar__link"><i class="myicon" data-feather="globe"></i><span>Кража персональных данных.</span></a>
    </li>
    <li class="navbar__item">
      <a href="Утечки данных..html" class="navbar__link"><i class="myicon" data-feather="smile"></i><span>Утечки данных.</span></a>        
    </li>
    <li class="navbar__item">
      <a href="Вредоносные программы и вирусы..html" class="navbar__link"><i class="myicon" data-feather="umbrella"></i><span>Вредоносные программы и вирусы.</span></a>        
    </li>
    <li class="navbar__item">
      <a href="Фишинговые и мошеннические электронные письма..html" class="navbar__link"><i class="myicon" data-feather="sun"></i><span>Фишинговые и мошеннические электронные письма.</span></a>        
    </li>
    <li class="navbar__item">
      <a href="Мошеннические сайты.html" class="navbar__link"><i class="myicon" data-feather="star"></i><span>Мошеннические сайты.</span></a>        
    </li>
    <li class="navbar__item">
      <a href="Интернет-мошенничество..html" class="navbar__link"><i class="myicon" data-feather="moon"></i><span>Интернет-мошенничество.</span></a>        
    </li>
    <li class="navbar__item">
      <a href="Кибербуллинг..html" class="navbar__link"><i class="myicon" data-feather="github"></i><span>Кибербуллинг.</span></a>        
    </li>
    <li class="navbar__item">
      <a href="Неверные настройки конфиденциальности..html" class="navbar__link"><i class="myicon" data-feather="key"></i><span>Неверные настройки конфиденциальности.</span></a>        
    </li>
  </ul>
</nav>
  <script src='https://unpkg.com/feather-icons'></script><!--Библиотека иконок-->
    <script id="rendered-js" >
    feather.replace();
    </script> 
        <p>Каждый современный человек, ежедневно проводит время в интернете. Но интернет — это не только источник информации и возможность общаться на расстояние, но и угроза компьютерной безопасности. Вы можете скачать из сети компьютерный вирус, Вашу учетную запись или адрес электронной почты могут взломать злоумышленники.<br>
        <br>
        Российская аудитория интернета стремительно растет – дети, подростки, молодежь составляют ее значительную часть. Сейчас уже почти каждый третий ребенок в нашей стране выходит в интернет, и чем старше подростки, тем выше среди них доля «интернетчиков». Сегодня детям доступно то, что лет пятнадцать назад было под силу лишь профессионалу или даже государству – создать собственную телестудию, получить картинку или музыку из-за тридевяти земель, поуправлять собственным мультфильмом. Во «взрослом» интернете, кроме этого, осуществляют платежи, потребляют электронные госуслуги, производят и продают контент. Через интернет дети и подростки открывают для себя мир, формируют собственную личность. Интернет дает пользователю огромные возможности как высокотехнологичный источник коммуникации, как инструмент поиска и получения информации. Для того чтобы эффективно использовать этот инструмент, нужны как умения обращаться с ним, так и определенный жизненный опыт, позволяющий не захлебнуться в океане неограниченных возможностей интернета, вовремя разглядеть подводные камни, рифы и водовороты виртуального пространства. С развитием интернета резко возросло число тех, кто использует его возможности в неблаговидных целях. Хорошо знакомые следователям и гражданам виды преступлений перешли в сеть, появились новые виды преступлений, порожденные интернетом. </p>
        <center>
        <h1 class="h1">Правила безопасности в интернете.</h1> <br>
        </center>
        <h3>1) Используйте надежный пароль. Первое и главное правило сохранности Ваших данных, учетных записей, почтовой пересылки это надежный пароль! Много раз хакеры взламывали страницы в социальных сетях или почтовые адреса из-за того, что пользователь ставил простой пароль. Вы ведь не хотите, чтобы Вашу личную переписку узнал кто-то чужой? Используйте генератор паролей, чтобы получить надежный пароль.
        Генератор паролей создается, чтобы помочь вам с придумыванием устойчивых к взлому и легко запоминающихся паролей.
        Часто бывает: вы зарегистрировались где-нибудь, а там просят: «введите пароль». В спешке приходится вводить что-нибудь типа qwerty или 12345. Последствия могут быть фатальными для вашего аккаунта: при попытке взлома такие пароли проверяются в первую очередь. Чтобы этого не происходило, надо создавать сложный пароль, желательно состоящий из букв разного регистра и содержащий цифры и другие символы.
        Для создания таких паролей существуют специальные программы. Но, на наш взгляд, гораздо легче набрать наш адрес и просто выбрать понравившийся пароль.</h3> <br>
        <h2 class="h2">Советы:</h2> <br>
              <ul>
                <li>   •  Выбирайте пароль посложнее, состоящий из символов разного регистра, с цифрами и для абсолютной надёжности - знаками препинания.</li> 
                <br>
                <li>   •  Не используйте пароль, связанный с теми данными, которые могут быть о вас известны, например, ваше имя или дату рождения.</li> 
                <br>
                <li>   •  Пароли, которые вы видите на экране создаются в реальном времени на вашем компьютере, поэтому исключена возможность перехвата пароля по  сети. Разные посетители сайта видят разные пароли. Если вы зайдете на сайт второй раз, пароли будут другими.</li> 
                <br>
                <li>   •  Вы можете выбрать пункт меню браузера "Файл|Сохранить как...", чтобы пользоваться генератором паролей в оффлайне.</li> 
                <br>
                <li>   •  Генератор паролей полностью прозрачен: скачайте файл passwd.js, чтобы увидеть, как создается пароль, и убедиться в абсолютной надежности.</li> 
            </ul>
            </div> <br> <br>
        <h3>2) Заходите в интернет с компьютера, на котором установлен фаервол или антивирус с фаерволом. Это в разы уменьшит вероятность поймать вирус или зайти на вредоносный сайт.<br>
        <br>
        3) Заведите один основной почтовый адрес и придумайте к нему сложный пароль. При регистрации на форумах, в соц. сетях и прочих сервисах Вы будете указывать его. Это необходимо если Вы забудете пароль или имя пользователя. Ни в коем случае не говорите, никому свой пароль к почте, иначе злоумышленник сможет через вашу почту получить доступ ко всем сервисам и сайтам, на которых указан Ваш почтовый адрес.<br>
        <br>
        4) Если Вы хотите скачать какой-то материал из интернета, на сайте где не нужна регистрация, но от Вас требуют ввести адрес своей электронной почты, то, скорее всего, на Ваш адрес будут высылать рекламу или спам. В таких случаях пользуйтесь одноразовыми почтовыми ящиками.<br>
        <br>
        5) Скачивайте программы либо с официальных сайтов разработчиков. Не скачивайте программы с подозрительных сайтов или с файлообменников. Так Вы уменьшите риск скачать вирус вместо программы.<br>
        <br>
        6) Не нажимайте на красивые баннеры или рекламные блоки на сайтах, какими бы привлекательными и заманчивыми они не были. В лучшем случае, Вы поможете автору сайта получить деньги, а в худшем — получите вирус. Используйте плагины для браузеров, которые отключают рекламу на сайтах.<br>
        <br>
        7) Если Вы работаете за компьютером, к которому имеют доступ другие люди (на роботе или в интернет кафе), не сохраняйте пароли в браузере. В противном случае, любой, кто имеет доступ к этому компьютеру, сможет зайти на сайт, используя Ваш пароль.<br>
        <br>
        8) Не открывайте письма от неизвестных Вам пользователей (адресов). Или письма с оповещением о выигрыше в лотереи, в которой Вы просто не участвовали.<br>
        <br>
        9) Не нажимайте на вплывающие окна, в которых написано, что Ваша учетная запись в социальной сети заблокирована. Это проделки злоумышленников! Если Вас вдруг заблокируют, Вы узнаете об этом, зайдя в эту социальную сеть, или администрация отправит Вам электронное письмо.<br>
        <br>
        10) Периодическим меняйте пароли на самых важных сайтах. Так Вы уменьшите риск взлома вашего пароля.</h3>
        <center><br>
        <h2 class="h2">Пользуясь этими правилами безопасности в интернете, Вы существенно уменьшите риск получить вирус на свой компьютер или потерять учетную запись на любимом сайте.</h2><br><br>
        <img src="images\3cf612c9-a26d-5eeb-8933-607247c9f37c.jpeg"alt='Картинка' width="420" height="230" style="position: relative; margin-bottom: -21px; border-radius: 10px;"><br>        
        <br><br>
        <footer>
          <h4 class="end">2025</h4><br>
        </footer>
        </center>
</body>
</html> <!--Главная страница готова-->
