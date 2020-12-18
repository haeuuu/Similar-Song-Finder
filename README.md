# 🎵 Similar Song Finder
### Song Finder 요새 꽂힌 그 노래와 비슷한 노래가 궁금해 !
> Goal : Melon의 유사곡 찾기 따라잡기 😎  

query곡과 유사한 곡 상위 10개를 골라 추천하고 멜론 링크를 제공합니다.
* Trie를 이용하여 50만개의 곡 중 query곡을 빠르게 탐색할 수 있도록 구현하였습니다.
  27만개의 곡을 for문으로 탐색하는 데에 약 0.07초, trie를 이용하면 약 0.01초가 소요됩니다.
* [Melon-playlist-generater Repository](https://github.com/haeuuu/Melon-playlist-generater)와 연결하여 자동으로 멜론 플레이 리스트에 추가할 수 있도록 구현할 수 있습니다.    
  
## 기능
##### 추천받고 싶은 곡 명을 입력하면, 어떤 곡인지 선택할 수 있습니다.
동명의 곡이 여러 곡인 경우, 여러 버전이 있는 경우에도 사용자가 원하는 곡을 제대로 찾을 수 있도록 합니다.
* 여러개의 곡 중 어느 곡인지 사용자에게 선택하도록 요구합니다.  
  
![example_오마이걸_비밀정원](fig/example_오마이걸_비밀정원.jpg)
* 만약 곡이 유일한 경우, 사용자에게 선택을 요구하지 않고 바로 추천 결과를 띄웁니다.  
  
![example_검정치마_나랑아니면](fig/example_검정치마_나랑아니면.jpg)
* 만약 DB에 등록되지 않은 곡이라면, 아무 노래나 랜덤으로 골라 추천하고 멜론 링크를 제공합니다.  
  
![example_unknown_songs](fig/example_unknown_songs.jpg)
  
    
##### 가장 유사한 곡 top 10과 멜론 링크를 제공합니다.
query 곡과 가장 유사한 상위 10곡을 추천하고, 10곡 중 한 곡을 랜덤으로 골라 멜론에서 들어볼 수 있도록 링크를 제공합니다.