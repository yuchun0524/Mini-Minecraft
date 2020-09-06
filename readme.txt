一、How to play your game
1、WASD控制人物移動，加shift可奔跑，空白鍵可跳躍
2、Y播放bgm、T暫停bgm，U切換bgm
3、左鍵可收集物品、消除怪物，想要產生inventory內的物品要先點選inventory內該物品再點右鍵
4、按c可切換視角(3段式)
5、q鍵、e鍵可以做人物旋轉
6、k鍵加速日夜轉換，搭配shift會更快速
7、p鍵回選單
注意事項：只有一開始的選單是用點擊的，後面出現的選單開始是S，暫停或繼續是P，結束是E

二、work distribution chart 
簡毓君：UI/UX Design、Map Design、Inventory Design

吳仰航：Character Design 、Game flow Control、Animation / Effect Design

三、Your game flow
一開始的選單有三個選項，分別是開始、暫停(繼續)和離開，進入遊戲後會自動生成物品，
點左鍵可收集物品，有三種物品可收集(cube)，
點inventory內物品再點右鍵可產生物品。
每50秒會做日夜轉換，夜晚時會有怪物出現並攻擊主角，可以左鍵點擊怪物來消除怪物或是躲進房子避免被攻擊(只有一棟有此效果)，
主角血量為8，每一次被怪物攻擊都會減一，血量沒了之後就會出現選單讓使用者決定要不要重新開始。


四、Game design (how to design your character, monster, etc.)
1、inventory
	inventory由panel和9個image組成，panel當作背景，9個image當作slot，每次要放進物品的時候，會在slot底下創image，
	這個新創的image用來放物品的sprite。有預先設計好的database，用來放哪些物品可以被放進inventory，
	每個要放進來的物品的sprite會預先存在resources的資料夾裡，每次放物品進來的時候就會去抓sprite。
2、character
	人物採用維京人當作角色，可以使用(wsad)鍵去進行角色之移動，使用shift搭配可以快速移動，
	空白鍵為跳躍，每個按鍵都會有相對應的動作與音效。
3、monster
	怪物有三個狀態，當人物太遠時會呈現休息狀態，當人物靠近則會去追擊主角，當主角與怪物有接觸時則怪物會進行攻擊，
	若是主角沒擊殺怪物或是快速離開，則開始降低血量(支援多重圍毆)。
4、day and night
	模擬真實太陽的運行軌跡(東升西落)，並且提供金手指(k鍵)去加快太陽的移動速度，搭配shift會更加快速，使得太陽出來讓怪物死亡。

五、Bonus
1、Inventory system可拖曳物品
2、Inventory system可根據物品剩餘數量來產生物品並根據點擊的物品而產生相對應的物品
3、怪物可以同時圍毆主角
4、qe鍵可以做人物旋轉
5、p鍵可以暫停遊戲叫出選單並支援繼續遊戲功能(S開始、P繼續、E離開)
6、c鍵三種視角切換(第一、第三、上帝視角)
7、k鍵可加快時間，加速天亮讓怪物死亡
8、太陽模擬真實的運作(東升西落)
9、U鍵可切換不同bgm、收集物品和消除怪物有音效
10、玩家掉落會出現選單方便使用者重來

六、Feedback
1、希望在講transform、gameobject、component的時候能夠更清楚、更詳細一點。
2、希望最後的homework可以簡單一點，可以讓我們有更多時間做final project。
