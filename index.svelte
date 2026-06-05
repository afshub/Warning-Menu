<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/rfl890/inter-cdn@3.19/inter.min.css">
<div class="backgr">
    <div class="warning-text">ПРЕДУПРЕЖДЕНИЕ</div>
    <div class="main-text"><span style="color: #C92A3F;">Администрация сервера никогда не требует передачи игрового имущества, валюты или предметов!</span> <span style="color: #818888;">Все сделки могут и должны совершаться через доступный функционал сервера.</span></div>
    <div class="infoblokback">
        <div class="info-text">Устные и другие договоренности не защитят Ваше игровое имущество.</div>
    </div>
    <label class="checkbox-container">
        <input type="checkbox" id="scales" name="scales" />
        <span class="checkmark"></span>
        <div class="dontshow-text">Больше не показывать</div>
    </label>
    <div class="skip" on:click={() => skip()}>
        <div class="skip-text">Принять и продолжить</div>
    </div>
</div>

<style>
.skip {
    position: absolute;
    width: 34.2vw;
    height: 5.5vh;
    bottom: 3.2vh;
    left: 1.9vw;
    background: #2A2A2A;
    border-radius: 0.5vh;
}

.skip:hover {
    background: #414141;
}

.skip-text {
    position: absolute;
    width: 10.7vw;
    height: 2.3vh;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 1.6vh;
    line-height: 2.3vh;
    letter-spacing: 0.025em;
    color: #FFFFFF;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.backgr {
    position: absolute;
    width: 38vw;
    height: 41.6vh;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background: #121212;
    border-radius: 1vh;
}

.warning-text {
    position: absolute;
    width: 11.9vw;
    height: 2.5vh;
    top: 3.2vh;
    left: 1.9vw;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 800;
    font-size: 2.1vh;
    line-height: 2.5vh;
    letter-spacing: 0.005em;
    color: #FFFFFF;
}

.main-text {
    position: absolute;
    width: 29.9vw;
    height: 6.7vh;
    top: 9vh;
    left: 1.9vw;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 1.6vh;
    line-height: 2.3vh;
    letter-spacing: 0.025em;
}

.checkbox-container {
    position: absolute;
    top: 29vh;
    left: 1.9vw;
    display: flex;
    align-items: center; 
    gap: 0.8vw;      
    cursor: pointer;
    user-select: none;
}

.checkbox-container input {
    position: absolute;
    opacity: 0;
    cursor: pointer;
    height: 0;
    width: 0;
}

.checkmark {
    box-sizing: border-box;
    position: relative; 
    width: 2.3vh;    
    height: 2.3vh;
    background: #252525;
    border: 0.1vh solid #373737;
    border-radius: 0.5vh;
    flex-shrink: 0; 
}

.checkbox-container:hover .checkmark {
    background-color: #252525;
    border-color: #5B5B5B;
}

.checkbox-container:hover .dontshow-text {
    color: #ffffff;
}

.checkbox-container input:checked ~ .checkmark {
    background-color: #E81C5A;
    border-color: #E81C5A;
}

.infoblokback {
    position: absolute;
    width: 34.2vw;
    height: 6.5vh;
    top: 19vh;
    left: 1.9vw;
    background: linear-gradient(90deg, #191919 99.69%, #FFBE40 99.69%);
    border-radius: 0.7vh;
}

.info-text {
    position: absolute;
    top: 50%;
    left: 1.3vw;
    transform: translateY(-50%);
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 1.5vh;
    line-height: 1.8vh;
    letter-spacing: -0.015em;
    color: #FFFFFF;
}

.dontshow-text {
    position: relative;
    left: 0;    
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 1.4vh;
    line-height: 1.4vh;
    letter-spacing: 0.025em;
    color: #818888;
    transition: color 0.2s ease;
}
</style>