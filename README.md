![header](https://capsule-render.vercel.app/api?type=venom&height=230&color=gradient&text=Hello,%20World!&fontColor=eeeeee&stroke=222222&strokeWidth=2.5)
### 안녕하세요! 👋

현재 시각은 <span id="current-time"></span> 입니다.

<script>
function updateTime() {
  const now = new Date();
  const hours = now.getHours();
  let greeting = '';

  if (hours < 12) {
    greeting = '좋은 아침입니다!';
  } else if (hours < 18) {
    greeting = '즐거운 오후 되세요!';
  } else {
    greeting = '좋은 저녁 되세요!';
  }

  const timeElement = document.getElementById('current-time');
  timeElement.textContent = `${greeting} 현재 시간은 ${hours}시 ${now.getMinutes()}분입니다.`;
}

updateTime();
setInterval(updateTime, 60000); // 매 분마다 업데이트
</script>

