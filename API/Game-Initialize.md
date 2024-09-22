# Game initialize

## Request

获取一个游戏的初始化数据。

```bash
GET {BASE_URL}/v1/games/{GAME_ID}

Authorization: Bearer {JWT}
```

## Response

```json
{
	"code": "",
	"message": "",
	"data": {
		"game": "Game Model",
		"preloaderImgUrl": ".../preloader.svg",
		"config": {
			"minBet": 1,
			"maxBet": 10,
			"betChangeAmount": 1,
			"defaultBetAmount": 1,
			"defaultLines": "",
			"images_path": "",
			"lines": [
				[1,1,1,1,1],
				[0,0,0,0,0],
				....
			],
			"symbols": [
				{
					"filename": "xxx.png",
					"scatter": false,
					"wild": false,
					"free": false,
					"w1": 0,
					"w1t": "x",
					"w2": 0,
					"wt": "x",
					"w3": 2,
					"w3t": "x",
					"w4": 10,
					"w4t": "x",
					"w5": 20,
					"w5t":  "x",
					"idx": 0,
					"el": []
				},
				...
			],
			"reels": [
				[0,1,2,3,4,5,6,7],
				...
			],
			"syms": [
				".../x.png", ....
			],
			"paytable": [
				{
	 				"scatter": false,
        				"wild": false,
        				"w1": "",
        				"w2": "",
        				"w3": "x2",
        				"w4": "x10",
        				"w5": "x20",
				},
				...
			],
			"free_games": [],
			"animation": "../animation.svg",
			"animation_color_border": "red",
			"animation_color_fill": "yellow",
			"animation_frames"  : 14,
                     "animation_time"    : 28,
                     "animation_size"    : 28.6,
                     "sym_size"          : 200,
                     "speed_max"         : 5000

		},
		"routes": {
			"play": "/game/play"
		},
		"sounds": {
			"click" :'audio/games/slots/click.wav',
			"lose" :'audio/games/slots/lose.wav',
			"spin" :'audio/games/slots/spin.wav',
			"start" :'audio/games/slots/start.wav',
			"stop" :'audio/games/slots/stop.wav',
			"win" :'audio/games/slots/win.wav',	
		}


	}
}
```
