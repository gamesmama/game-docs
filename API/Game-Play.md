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
		"gameable_id": 105,
		"bet": 10,
		"win": 0,
		"status": 1,
		"client_seed": 332091,
		"created_at": "2024-09-24T13:53:25.000000Z",
		"updated_at": "2024-09-24T13:53:36.000000Z",
		"next_game": {
			"account_id": 2,
			"bet": 0,
			"win": 0,
			"status": -1,
			"gameable_id": 106,
			"updated_at": "2024-09-24T13:53:36.000000Z",
			"created_at": "2024-09-24T13:53:36.000000Z",
			"id": 106,
			"server_hash": "13589cf96c35ed3bebe86154fe160eb46db00135948effd978db8b1a9370aec3",
			"account": {
			"id": 2,
			"user_id": 2,
			"balance": 50870,
			"created_at": "2024-06-26T08:09:09.000000Z",
			"updated_at": "2024-09-24T13:53:25.000000Z"
			}
		},
		"server_hash": "d93c1bedca2987fdbae1e590821e0d6ea55bf031850ead8c5d9579c33e594e9b",
		"gameable": {
			"id": 105,
			"lines_bet": 10,
			"bet_amount": 1,
			"lines_win": 0,
			"scatters_count": 0,
			"free_games_count": 0,
			"reel_positions": "7,1,7,3,1",
			"game_index": "1",
			"created_at": "2024-09-24T13:53:25.000000Z",
			"updated_at": "2024-09-24T13:53:36.000000Z",
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
			"win_lines_ttl": [],
			"win_lines": []
		},
		"account": {
			"id": 2,
			"user_id": 2,
			"balance": 50860,
			"created_at": "2024-06-26T08:09:09.000000Z",
			"updated_at": "2024-09-24T13:53:25.000000Z",
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
			"updated_at": "2024-09-19T15:21:13.000000Z"
			}
		}
	}
}
```
