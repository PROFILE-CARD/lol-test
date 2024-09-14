# REQUEST HEADER

```
{
    "X-Riot-Token": "RGAPI-6179a6bc-7c63-4c68-8e6f-9d1a4e629b79"
}
```

# STEP.1

`https://asia.api.riotgames.com/riot/account/v1/accounts/by-riot-id/{gameName}/{tagLine}`

`https://asia.api.riotgames.com/riot/account/v1/accounts/by-riot-id/%EC%A5%AC%EC%94%A8%EB%AC%BC%EC%A1%B0%EC%A0%88%EC%9E%A5%EC%9D%B8/KR1`

```
{
    "puuid": "QH5h5X8N15ObAcAQ00ohOWp3-eY1d4XAVOhtFdTCwGrVP_KCGllWdEIzu4M5QAkgw8zcCq5-U2fAWQ",
    "gameName": "쥬씨물조절장인",
    "tagLine": "KR1"
}
```

# STEP.2

`https://kr.api.riotgames.com/lol/summoner/v4/summoners/by-puuid/{puuid}`

`https://kr.api.riotgames.com/lol/summoner/v4/summoners/by-puuid/QH5h5X8N15ObAcAQ00ohOWp3-eY1d4XAVOhtFdTCwGrVP_KCGllWdEIzu4M5QAkgw8zcCq5-U2fAWQ`

```
{
    "id": "IhUMj1Qb0G3fbtFauSzti2vDjGPkXf6uhbF8xrVOV6MRNA",
    "accountId": "s3FB7gux2o2LYVJqZbJ2mqqUmV2NgAOf42SL-ztFh8-u",
    "puuid": "QH5h5X8N15ObAcAQ00ohOWp3-eY1d4XAVOhtFdTCwGrVP_KCGllWdEIzu4M5QAkgw8zcCq5-U2fAWQ",
    "profileIconId": 6504,
    "revisionDate": 1726256495429,
    "summonerLevel": 362
}
```

# STEP.3

`https://kr.api.riotgames.com/lol/league/v4/entries/by-summoner/{id}`

`https://kr.api.riotgames.com/lol/league/v4/entries/by-summoner/IhUMj1Qb0G3fbtFauSzti2vDjGPkXf6uhbF8xrVOV6MRNA`

```
[
    {
        "leagueId": "c910b111-3b84-47d6-bcad-5b1493c62ba2",
        "queueType": "RANKED_FLEX_SR",
        "tier": "EMERALD",
        "rank": "III",
        "summonerId": "IhUMj1Qb0G3fbtFauSzti2vDjGPkXf6uhbF8xrVOV6MRNA",
        "leaguePoints": 20,
        "wins": 72,
        "losses": 69,
        "veteran": false,
        "inactive": false,
        "freshBlood": false,
        "hotStreak": false
    },
    {
        "leagueId": "a9efcb6f-ab5d-4fd8-b64b-3dc1c29cd06b",
        "queueType": "RANKED_SOLO_5x5",
        "tier": "EMERALD",
        "rank": "IV",
        "summonerId": "IhUMj1Qb0G3fbtFauSzti2vDjGPkXf6uhbF8xrVOV6MRNA",
        "leaguePoints": 0,
        "wins": 13,
        "losses": 21,
        "veteran": false,
        "inactive": false,
        "freshBlood": true,
        "hotStreak": false
    }
]
```
