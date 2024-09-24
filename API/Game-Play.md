# Game Play

## Request

```bash
POST {BASE_URL}/v1/games/{GAME_ID}

Authorization: Bearer {JWT}

{
    "seed": 488107,
    "lines_count": 10,
    "bet": 1
}
```


## Response

```JSON
{
	"code": "",
	"message": "",
	"data": {
    "account_id": 2,
    "gameable_id": 107,
    "bet": 10000,
    "win": 5000,
    "status": 1,
    "client_seed": 689110,
    "created_at": "2024-09-24T13:56:06.000000Z",
    "updated_at": "2024-09-24T13:56:39.000000Z",
    "next_game": {
        "account_id": 2,
        "bet": 0,
        "win": 0,
        "status": -1,
        "gameable_id": 108,
        "updated_at": "2024-09-24T13:56:39.000000Z",
        "created_at": "2024-09-24T13:56:39.000000Z",
        "id": 108,
        "server_hash": "338dfbf88022e100ec874049ed140ad371626173691e7f82468898602d3d58e2",
        "account": {
			"id": 2,
			"user_id": 2,
			"balance": 50842,
			"created_at": "2024-06-26T08:09:09.000000Z",
			"updated_at": "2024-09-24T13:56:06.000000Z"
        	}
    	},
	"server_hash": "8eba162465da213276041d799f74ea8a504b5295a561a395c86727d867398159",
	"gameable": {
		"id": 107,
		"lines_bet": 20,
		"bet_amount": 500,
		"lines_win": 2,
		"scatters_count": 0,
		"free_games_count": 0,
		"reel_positions": "1,1,7,4,3",
		"game_index": "1",
		"created_at": "2024-09-24T13:56:06.000000Z",
		"updated_at": "2024-09-24T13:56:39.000000Z",
		"win_scatters_ttl": 0,
		"win_scatters": [
		[],
		[],
		[],
		[],
		[]
		],
		"free_games_quantity": 0,
		"win_free_games": [
		[],
		[],
		[],
		[],
		[]
		],
		"is_free_game": false,
		"win_lines_ttl": {
		"5": 2500,
		"6": 2500
		},
		"win_lines": {
		"5": [
			2,
			1,
			0,
			null,
			null
		],
		"6": [
			2,
			1,
			0,
			null,
			null
		]
		}
	},
	"account": {
		"id": 2,
		"user_id": 2,
		"balance": 45842,
		"created_at": "2024-06-26T08:09:09.000000Z",
		"updated_at": "2024-09-24T13:56:06.000000Z",
		"user": {
		"id": 2,
		"name": "yao3060",
		"email": "yao3060@gmail.com",
		"referee_sign_up_credits": null,
		"referrer_sign_up_credits": null,
		"referrer_game_loss_pct": null,
		"referrer_game_win_pct": null,
		"referrer_deposit_pct": null,
		"last_login_at": "2024-09-19T15:21:13.000000Z",
		"email_verified_at": null,
		"created_at": "2024-06-26T08:09:09.000000Z",
		"updated_at": "2024-09-19T15:21:13.000000Z",
		"account": {
				"id": 2,
				"user_id": 2,
				"balance": 46342,
				"created_at": "2024-06-26T08:09:09.000000Z",
				"updated_at": "2024-09-24T13:56:39.000000Z"
			}
		}
		}
	}
}
```
