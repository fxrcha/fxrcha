### 저는 이런걸 제일 좋아합니다.

```python
import streamlink
import subprocess

def returnM3U8_Azi():
  stream_obj = streamlink.streams ("https://twitch.tv/dkwl025")
  link = stream_obj["best"].url
  return link

def startFFmpeg():
  m3u8_link = returnM3U8_Azi()
  cmd = [
       "ffmpeg",
       "-i", m3u8_link,
       "-c", "copy",
       "-map_metadata", "0",
       "술주정한거는_친구한테_부산의호떡을.mkv"
   ]
   process = subprocess.Popen(
       cmd,
       stdout=subprocess.PIPE,
       stderr=subprocess.PIPE,
   )
   print (f"Starting Something : {process.pid}")

if __name__ == "__main__":
  startFFmpeg()
```

### 아니면 이딴거요.

```cpp
#include <bits/stdc++.h>
using namespace std;
int dp[5386], n;

int main () {
  ios_base::sync_with_stdio(false);
  cin.tie(0);
  cout.tie(0);
  cin >> n;
  dp[0] = 0, dp[1] = 1;
  for (int i = 2; i <= n; ++i) dp[i] = dp[i - 1] + dp[i - 2]:
  cout << dp[n];
  return 0;
}
```

### 그리고 씨잼은 하루빨리 앨범을 내야합니다.
살면서 누구앨범 뒤지게 기다려본적은 없네 성민이형
제발 앨범좀 내주면 안될까? 오예 어디같이 정식이 
아니여도 돼,, 불러 같은 싱글도 괜찮으니깐
제발 이번년도에는 형의 앨벙믈 보고싶어..
수수께기 화난여자 미공개곡도 많잖아..
알겠지 형?

![그의 업적](https://github-readme-stats.vercel.app/api?username=fxrchal&show_icons=true)
