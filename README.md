# Study_DNS_Mapping

## [GitHub과 DOTHOME DNS Mapping하기]
*****
### 1. Repository Settings
<pre><code>1. Repository에서 Settings를 클릭하여 Settings 페이지로 갑니다.
2. 페이지 하단에서 GitHub Pages 영역의 Source 부분을 수정해 줍니다.
- master branch의 소스를 사용하겠습니다.
3. 새로고침이 되면 다시 하단 GitHub Pages 영역의 Custom domain 작성란에 도메인 네임을 넣고 Save해줍니다.</code></pre>

### 2. GitHub IP 복사하기
<pre><code>1. Custom domain 영역의 설명글에 있는 링크 (Learn more)을 클릭합니다.
2. 이동 된 페이지에서 setting up an apex domain을 검색해서 클릭하여 페이지 이동을 합니다.
3. 페이지에서 Configuring A records with your DNS provider 를 검색합니다.
4. IP를 확인합니다.</code></pre>

### 3. DNS 호스팅 설정
<pre><code>1. DOTHOME 사이트에서 '마이닷홈'을 눌러 사용자 페이지로 이동합니다.
2. DNS관리 > DNS 레코드 관리 > 레코드 추가 해줍니다.
- Type은 클릭 시 설명이 나옵니다. A Type을 눌러줍니다. (A Type은 도메인에 실 서버 IP를 설정하는 것이라고 합니다)
- 도메인 네임은 git에서 지정한 네임을 입력해줍니다.(지정하는 도메인이 정해져 있길래 DOTHOME 룰에 따랐습니다)
- TTL 값을 지정해줍니다.
-- TTL(Time to Live), 캐싱 데이터의 유효기간이라고 합니다.
--- 위키디피아 : https://ko.wikipedia.org/wiki/Time_to_live
--- 생활코딩 : https://opentutorials.org/course/697/3839 ttl을 검색해보세요! ttl과 캐싱에 대한 설명이 있습니다.
3. GitHub의 IP를 값 영역에 넣어줍니다.
- 다 등록해도되고 하나만 해도 되는데, 여러개 등록할 경우 해당 서버에 이상이 생겼을 경우 이상이 없는 서버로 연결이 가능하다고 합니다.
4. 추가하기를 눌러 해당 도메인으로 접근해봅니다.
5. 수정하여 반영이 된 것을 확인합니다.
- 실시간 반영은 아닌 것 같고 약간의 시간차가 생기는것으로 확인했습니다.</code></pre>
