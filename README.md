
python3 -m http.server


## love running project
## https://jacobheflin.com/#about
## bootstrap
## W3schools.com
## Traversy Media youtube tutorial



### contact bg img Image by <a href="https://pixabay.com/users/geralt-9301/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2944064">Gerd Altmann</a> from <a href="https://pixabay.com/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2944064">Pixabay</a>






.skills-container {
  position: relative;
  display: flex;
  justify-content: space-around;
}

.skills-container .card {
  position: relative;
  width: 200px;

  display: flex;
  justify-content: center;
  align-items: center;
  height: 300px;

  text-align: center;
  overflow: hidden;
  transition: 0.5s;
}

.box {
  position: relative;
  width: 300px;
  height: 400px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  background: #fff;
  box-shadow: 0 30px 60px rgba(76, 85, 88, 0.2);
}

.box .percent {
  position: relative;
  width: 150px;
  height: 150px;
}

.box .percent svg {
  position: relative;
  width: 150px;
  height: 150px;
}

.box .percent svg circle {
  width: 100px;
  height: 100px;
  fill: none;
  stroke-width: 10;
  stroke: #000;
  stroke-linecap: round;
  transform: translate(5px, 5px);
  stroke-dasharray: 440;
  stroke-dashoffset: 440;
}

.box .percent svg circle:nth-child(1) {
  stroke-dashoffset: 0;
  stroke: #f3f3f3;
}

.box .percent svg circle:nth-child(2) {
  stroke-dasharray: 440;
  stroke-dashoffset: 440;
  stroke: yellow;
  opacity: 1;
  animation: animate-circle 2s cubic-bezier(0, 0.23, 1, 0.1);
}

.card:nth-child(1) .box .percent svg circle:nth-child(2) {
  stroke-dashoffset: calc(440 - (440 * 60) / 100);
  stroke: yellow;
  opacity: 1;
  animation: animate-circle 2s cubic-bezier(0, 0.23, 1, 0.1);
}

.card:nth-child(2) .box .percent svg circle:nth-child(2) {
  stroke-dashoffset: calc(440 - (440 * 50) / 100);
  stroke: yellow;
  opacity: 1;
  animation: animate-circle 2s cubic-bezier(0, 0.23, 1, 0.1);
}
.card:nth-child(3) .box .percent svg circle:nth-child(2) {
  stroke-dashoffset: calc(440 - (440 * 40) / 100);
  stroke: yellow;
  opacity: 1;
  animation: animate-circle 2s cubic-bezier(0, 0.23, 1, 0.1);
}

.card:nth-child(4) .box .percent svg circle:nth-child(2) {
  stroke-dashoffset: calc(440 - (440 * 60) / 100);
  stroke: yellow;
  opacity: 1;
  animation: animate-circle 2s cubic-bezier(0, 0.23, 1, 0.1);
}

.card:nth-child(5) .box .percent svg circle:nth-child(2) {
  stroke-dashoffset: calc(440 - (440 * 70) / 100);
  stroke: yellow;
  opacity: 1;
  animation: animate-circle 2s cubic-bezier(0, 0.23, 1, 0.1);
}

.card:nth-child(6) .box .percent svg circle:nth-child(2) {
  stroke-dashoffset: calc(440 - (440 * 50) / 100);
  stroke: yellow;
  opacity: 1;
  animation: animate-circle 2s cubic-bezier(0, 0.23, 1, 0.1);
}

.box .percent .number {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #999;
}

.box .percent .number h2 {
  font-size: 48px;
}

.box .percent .number h2 span {
  font-size: 24px;
}

.box .text {
  padding: 10px 0 0;
  color: #999;
  font-weight: 700;
  margin-top: 20px;
  text-transform: uppercase;
}

@keyframes animate-circle {
  30% {
    opacity: 0.3;
    stroke-dashoffset: 350;
  }
  50% {
    opacity: 0.5;
    stroke-dashoffset: 150;
  }
  100% {
    opacity: 1;
  }
}
