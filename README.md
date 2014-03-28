Vizoal API
==================================================

Global Path: http://api.vizoal.com

```
Player Image：  /vizoal/image/android/player/2.0/{player_fm_id}.png
Club Image：    /vizoal/image/android/club_logo/2.0/{club_fm_id}.png
Country Image： /vizoal/image/android/country_logo_profile/2.0/{country_fm_id}.png
League Image：  /vizoal/image/android/league/{league_fm_id}.png
```

##APIs
<ol>
<li> Get Top players </li>
<li> Get players by club id</li>
<li> Get clubs by league id</li>
<li> Get player profile by player id </li>
<li> Get homepage players </li>
<li> Search </li>
<li> Create an account </li>
<li> Update an account </li>
<li> Login </li>
<li> Post a comment </li>
<li> Get comment list by player id </li>
<li> Get old comment list by player id </li>
<li> Get player statistics </li>
<li> country logo url </li>
<li> Top League List </li>

</ol>

##1 : Get popular players
------------------------
###URL
        /vizoal/services/playerlist/1  
           
###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
	
###Image URL			
	/vizoal/image/android/player/3.0/{player_fm_id}.png

###JSON Response
```
{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ip-172-31-15-220",
            "duration": 6
        }
    },
    "result": [
        {
            "playerId": 2055,
            "firstName": "Joe",
            "lastName": "Mason",
            "fullName": "Joseph Mason",
            "nickName": "",
            "nationOfBirth": 122,
            "nationDisplay": 103,
            "nationOfBirthName": "Republic of Ireland",
            "cityOfBirth": "Plymouth",
            "dateOfBirth": "1991-05-13",
            "nationDisplay_fmid": 789,
            "age": 0,
            "weight": "73",
            "height": "178",
            "preferFoot": "right",
            "currentClub": 44,
            "currentClubName": "Cardiff City",
            "clubNumber": "20",
            "fmId": 28017168,
            "version": 3
        },
        {
            "playerId": 2066,
            "firstName": "Darcy",
            "lastName": "Blake",
            "fullName": "Darcy James Blake",
            "nickName": "",
            "nationOfBirth": 116,
            "nationDisplay": 116,
            "nationOfBirthName": "Wales",
            "cityOfBirth": "New Tredegar",
            "dateOfBirth": "1988-12-13",
            "nationDisplay_fmid": 801,
            "age": 0,
            "weight": "79",
            "height": "178",
            "preferFoot": "right",
            "currentClub": 46,
            "currentClubName": "Crystal Palace F.C.",
            "clubNumber": "",
            "fmId": 5131839,
            "version": 2
        }
    ]
}
```

##2 : Get players by club id
------------------------
###URL
        /vizoal/services/playerlistByClub/{clubId}  
           
###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
	
###Image URL			
	Player Image：	/vizoal/image/android/player/2.0/{player_fm_id}.png
	

###JSON Response Sample
```
{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ip-172-31-15-220",
            "duration": 145
        }
    },
    "result": [
        {
            "playerId": 94,
            "firstName": "Santi",
            "lastName": "Cazorla",
            "fullName": "Santiago Cazorla González",
            "nickName": "",
            "nationOfBirth": 90,
            "nationDisplay": 90,
            "nationOfBirthName": "Spain",
            "cityOfBirth": "Lugo De Llanera",
            "dateOfBirth": "1984-12-13",
            "nationDisplay_fmid": 796,
            "age": 0,
            "weight": "66kg",
            "height": "168",
            "preferFoot": "either",
            "currentClub": 16,
            "currentClubName": "Arsenal",
            "clubNumber": "19",
            "fmId": 7456688,
            "version": 2,
            "playerPositionList": [
                {
                    "playerPositionId": 312,
                    "playerId": 94,
                    "name": "AMC",
                    "efficiency": "100%",
                    "order": null,
                    "version": 2
                },
                {
                    "playerPositionId": 313,
                    "playerId": 94,
                    "name": "AML",
                    "efficiency": "90%",
                    "order": null,
                    "version": 1
                },
                {
                    "playerPositionId": 314,
                    "playerId": 94,
                    "name": "AMR",
                    "efficiency": "90%",
                    "order": null,
                    "version": 1
                },
                {
                    "playerPositionId": 315,
                    "playerId": 94,
                    "name": "ML",
                    "efficiency": "90%",
                    "order": null,
                    "version": 2
                },
                {
                    "playerPositionId": 316,
                    "playerId": 94,
                    "name": "MR",
                    "efficiency": "90%",
                    "order": null,
                    "version": 1
                },
                {
                    "playerPositionId": 317,
                    "playerId": 94,
                    "name": "MC",
                    "efficiency": "90%",
                    "order": null,
                    "version": 1
                }
            ]
        },
        {
            "playerId": 92,
            "firstName": "Francis",
            "lastName": "Coquelin",
            "fullName": "Francis Coquelin",
            "nickName": "",
            "nationOfBirth": 135,
            "nationDisplay": 135,
            "nationOfBirthName": "France",
            "cityOfBirth": "Laval",
            "dateOfBirth": "1991-05-13",
            "nationDisplay_fmid": 769,
            "age": 0,
            "weight": "73",
            "height": "178",
            "preferFoot": "right",
            "currentClub": 16,
            "currentClubName": "Arsenal",
            "clubNumber": "20",
            "fmId": 34012022,
            "version": 2,
            "playerPositionList": [
                {
                    "playerPositionId": 296,
                    "playerId": 92,
                    "name": "DMC",
                    "efficiency": "100%",
                    "order": null,
                    "version": 1
                },
                {
                    "playerPositionId": 297,
                    "playerId": 92,
                    "name": "MC",
                    "efficiency": "90%",
                    "order": null,
                    "version": 1
                },
                {
                    "playerPositionId": 298,
                    "playerId": 92,
                    "name": "DR",
                    "efficiency": "80%",
                    "order": null,
                    "version": 1
                },
                {
                    "playerPositionId": 299,
                    "playerId": 92,
                    "name": "DL",
                    "efficiency": "80%",
                    "order": null,
                    "version": 1
                },
                {
                    "playerPositionId": 300,
                    "playerId": 92,
                    "name": "WBR",
                    "efficiency": "80%",
                    "order": null,
                    "version": 1
                },
                {
                    "playerPositionId": 301,
                    "playerId": 92,
                    "name": "MR",
                    "efficiency": "80%",
                    "order": null,
                    "version": 1
                }
            ]
        }
    ]
}
```

##3 : Get clubs by league
------------------------
###URL 
        Right now just hard-coded for top 5 leagues:
        
        Barclays Premier League(England):  /vizoal/services/clublistByLeague/11  
        Bundesliga(Germany):               /vizoal/services/clublistByLeague/17  
        Ligue 1(France):                   /vizoal/services/clublistByLeague/21  
        Liga BBVA(Spain):                  /vizoal/services/clublistByLeague/19 
        Serie A(Italy):                    /vizoal/services/clublistByLeague/15  
           
###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
	
###Image URL			
	 /vizoal/image/android/club_logo/3.0/{club_fm_id}.png

###JSON Response Sample
```
{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ip-172-31-15-220",
            "duration": 9
        }
    },
    "result": [
        {
            "clubId": 33,
            "name": "West Bromwich Albion F.C.",
            "leagueId": 11,
            "fmId": 734,
            "sort": 0,
            "version": 1
        },
        {
            "clubId": 34,
            "name": "West Ham United F.C.",
            "leagueId": 11,
            "fmId": 735,
            "sort": 0,
            "version": 1
        }
    ]
}
```


##4 : Get player profile by player id
------------------------
###URL 
        /vizoal/services/player/{playerId}
           
###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
	
###Image URL			
	Player Image：  /vizoal/image/android/player/2.0/{player_fm_id}.png
	Club Image：    /vizoal/image/android/club_logo/2.0/{club_fm_id}.png
	Country Image： /vizoal/image/android/country_logo_profile/2.0/{country_fm_id}.png

###JSON Response Sample
```
{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ip-172-31-15-220",
            "duration": 54
        }
    },
    "result": {
        "playerId": 21,
        "firstName": "Ryan",
        "lastName": "Giggs",
        "fullName": "Ryan Joseph Giggs",
        "nickName": "",
        "nationOfBirth": 116,
        "nationDisplay": 116,
        "nationOfBirthName": "Wales",
        "cityOfBirth": "Cardiff",
        "dateOfBirth": "1973-11-29",
        "dateOfBirth_andriod": "November 29 1973",
        "age": 39,
        "weight": "69kg",
        "height": "180cm",
        "preferFoot": "left",
        "currentClub": 23,
        "currentClubName": "Manchester United F.C.",
        "fmId": 2018995,
        "nationality_fmid": 801,
        "club_fm_id": 680,
        "leagueId": 11,
        "leagueName": "Barclays Premier League",
        "version": 2,
        "playerPositionList": [
            {
                "playerPositionId": 48,
                "playerId": 21,
                "name": "AMC",
                "efficiency": "100%",
                "order": 1,
                "version": 1
            },
            {
                "playerPositionId": 49,
                "playerId": 21,
                "name": "AML",
                "efficiency": "90%",
                "order": 2,
                "version": 1
            },
            {
                "playerPositionId": 50,
                "playerId": 21,
                "name": "ML",
                "efficiency": "90%",
                "order": 3,
                "version": 1
            },
            {
                "playerPositionId": 51,
                "playerId": 21,
                "name": "MC",
                "efficiency": "90%",
                "order": 4,
                "version": 1
            },
            {
                "playerPositionId": 52,
                "playerId": 21,
                "name": "AMR",
                "efficiency": "70%",
                "order": 5,
                "version": 1
            },
            {
                "playerPositionId": 53,
                "playerId": 21,
                "name": "ST",
                "efficiency": "50%",
                "order": 6,
                "version": 1
            }
        ],
        "playerClubRecordList": [
            {
                "playerClubRecordId": 41,
                "clubId": 23,
                "clubName": "Manchester United F.C.",
                "playerId": 21,
                "seasonFrom": "1987-88",
                "seasonEnd": "1990-91",
                "previousClubId": null,
                "transferInfo": null,
                "youthStatus": "1",
                "loanFrom": null,
                "loanFromName": null,
                "coOwnWith": null,
                "coOwnWithName": null,
                "currentStatus": null,
                "order": 1,
                "version": 1
            },
            {
                "playerClubRecordId": 42,
                "clubId": 23,
                "clubName": "Manchester United F.C.",
                "playerId": 21,
                "seasonFrom": "1990-91",
                "seasonEnd": "Present",
                "previousClubId": null,
                "transferInfo": null,
                "youthStatus": "0",
                "loanFrom": null,
                "loanFromName": null,
                "coOwnWith": null,
                "coOwnWithName": null,
                "currentStatus": null,
                "order": null,
                "version": 1
            }
        ],
        "playerPlayerNationalityList": [
            {
                "playerNationalityId": 11,
                "playerId": 21,
                "nationalityId": 116,
                "name": "Wales",
                "abbreviation": "Welsh",
                "eligible": false,
                "isFirstTeam": true,
                "order": 1,
                "version": 3
            },
            {
                "playerNationalityId": 12,
                "playerId": 21,
                "nationalityId": 188,
                "name": "Sierra Leone",
                "abbreviation": "Sierra Leonian",
                "eligible": false,
                "isFirstTeam": true,
                "order": 2,
                "version": 4
            }
        ]
    }
}
```

##5 : Get homepage players
------------------------
###URL 
        /vizoal/services/player/homepage
           
###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
	
###Image URL 
```
Android:	
		/vizoal/image/android/homepage/hdRez/1.png
		/vizoal/image/android/homepage/hiRez/1.png
		/vizoal/image/android/homepage/medRez/1.png
		/vizoal/image/android/homepage/lowRez/1.png
	
IOS:		
		/vizoal/image/ios/homepage/iphone1/1.png
		/vizoal/image/ios/homepage/iphone2/1.png
		/vizoal/image/ios/homepage/iphone5/1.png
```

### Response
```

{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ip-172-31-15-220",
            "duration": 6
        }
    },
    "result": [
        {
            "playerId": 960,
            "name": "Lionel Messi",
            "image": "1.png"
        },
        {
            "playerId": 1205,
            "name": "Cristiano Ronaldo",
            "image": "2.png"
        },
        {
            "playerId": 0,
            "name": "Neymar",
            "image": "3.png"
        },
        {
            "playerId": 116,
            "name": "Wayne Rooney",
            "image": "4.png"
        }
    ]
}

```

##6: Search 
------------------------
###
###URL 
```
       /vizoal/services/search?keyword={keyword}&limit={limit}&offset={offset}
       
       Sample: /vizoal/services/search?keyword=Diego%20Mil&offset=0&limit=10
       
       offset: start from
       limit:  how many records per page
```
           
###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
 
### Response
```

{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ip-172-31-12-36",
            "duration": 26
        }
    },
    "result": {
        "totalCount": 5,
        "searchItemList": [
            {
                "type": "player",
                "playerId": 282,
                "playerName": "Ramírez Gastón",
                "playerFMId": 78027222,
                "clubId": 28,
                "clubName": "Southampton",
                "clubFMId": 713,
                "leagueId": null,
                "leagueName": "",
                "countryId": 93,
                "countryName": "Uruguay",
                "countryFMId": 1657
            },
            {
                "type": "player",
                "playerId": 1138,
                "playerName": "Demichelis Martín",
                "playerFMId": 952826,
                "clubId": 22,
                "clubName": "Manchester City",
                "clubFMId": 679,
                "leagueId": null,
                "leagueName": "",
                "countryId": 92,
                "countryName": "Argentina",
                "countryFMId": 1649
            },
            {
                "type": "player",
                "playerId": 1984,
                "playerName": "López Maxi",
                "playerFMId": 951030,
                "clubId": 77,
                "clubName": "Sampdoria",
                "clubFMId": 1167,
                "leagueId": null,
                "leagueName": "",
                "countryId": 92,
                "countryName": "Argentina",
                "countryFMId": 1649
            },
            {
                "type": "player",
                "playerId": 2145,
                "playerName": "Rubén Marco ",
                "playerFMId": 961949,
                "clubId": 129,
                "clubName": "Evian",
                "clubFMId": 3502354,
                "leagueId": null,
                "leagueName": "",
                "countryId": 92,
                "countryName": "Argentina",
                "countryFMId": 1649
            },
            {
                "type": "club",
                "playerId": null,
                "playerName": "",
                "playerFMId": null,
                "clubId": 17,
                "clubName": "Aston Villa",
                "clubFMId": 603,
                "leagueId": 11,
                "leagueName": "Premier League",
                "countryId": 122,
                "countryName": "England",
                "countryFMId": 765
            }
        ]
    }
}
```
 
##7 : Create an account  
------------------------
###Coming soon


##8 : Update an account  
------------------------
###Coming soon


##9 : Login  
------------------------
###Coming soon


##10 : Post a comment  
------------------------
###
###URL 
        /vizoal/services/playerComment
           
###Method			
	POST
				
###Header Parameters		
	1) Content-Type = application/json 

### Request
```
{
    "playerId": 14,
    "userName": "ethanchen",
    "comment": "fk222..............."
}
```

### Response

It will return new inserted player comment id

```

{
  "status": {
    "code": "200",
    "message": "success",
    "errors": [],
    "debug": {
      "build": "1.0",
      "serverName": "ethan",
      "duration": 1634
    }
  },
  "result": 135
}
```


##11 : Get latest comment list by player id  
------------------------

###  It will return the latest 15 records

###URL 
        /vizoal/services/playerComment/{playerId}
           
###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
 
### Response
```

{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ip-172-31-12-36",
            "duration": 14
        }
    },
    "result": {
        "totalCount": 8,
        "playerCommentList": [
            {
                "playerCommentId": 311,
                "playerId": 1205,
                "userName": "wert",
                "comment": "wow..........",
                "displayTime": "just now",
                "post_date": "2014-03-26 00:53:44"
            },
            {
                "playerCommentId": 310,
                "playerId": 1205,
                "userName": "wert",
                "comment": "ship i ship,,..................",
                "displayTime": "12 minutes ago",
                "post_date": "2014-03-26 00:41:05"
            },
            {
                "playerCommentId": 308,
                "playerId": 1205,
                "userName": "Jason",
                "comment": "test",
                "displayTime": "1 hours ago",
                "post_date": "2014-03-25 23:05:17"
            }
            ....................more
        ]
    }
}
```

##12 : Get old comment list by player id  
------------------------

###  It returns 15 records before given playerCommentId

###URL 
        /vizoal/services/playerComment/old/{playerId}/{lastPlayerCommentId}
       
       Example:  Suppose currently your page is displaying 30 records about player xxx, and the playerCommentids are 200,199,198.....170.
                 If you want to get 15 more earlier records about the player, the expected url is:
                 /vizoal/services/playerComment/old/xxx/170.   
###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
 
### Response
```

{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ethan",
            "duration": 437
        }
    },
    "result": [
        {
            "playerCommentId": 135,
            "playerId": 14,
            "userName": "ethanchen",
            "comment": "fk222...............",
            "post_date": "2013-11-20 20:08:42"
        },
        {
            "playerCommentId": 133,
            "playerId": 14,
            "userName": "unknown",
            "comment": "tredfgfcdf....again",
            "post_date": "2013-11-21 04:00:47"
        },
        {
            "playerCommentId": 132,
            "playerId": 14,
            "userName": "ethanchen",
            "comment": "fk222...............",
            "post_date": "2013-11-20 20:00:27"
        },
        {
            "playerCommentId": 131,
            "playerId": 14,
            "userName": "ethanchen",
            "comment": "fk...............",
            "post_date": "2013-11-20 19:56:10"
        },
        {
            "playerCommentId": 130,
            "playerId": 14,
            "userName": "ethanchen",
            "comment": "fk",
            "post_date": "2013-11-20 19:55:20"
        },
        {
            "playerCommentId": 125,
            "playerId": 14,
            "userName": "unknown",
            "comment": "tyy",
            "post_date": "2013-11-10 23:49:37"
        },
        {
            "playerCommentId": 79,
            "playerId": 14,
            "userName": "unknown",
            "comment": "",
            "post_date": "2013-10-28 06:28:09"
        },
        {
            "playerCommentId": 63,
            "playerId": 14,
            "userName": "unknown",
            "comment": "hello",
            "post_date": "2013-08-11 03:04:40"
        },
        {
            "playerCommentId": 62,
            "playerId": 14,
            "userName": "unknown",
            "comment": ".%46#%$&%%#$$%%$$&%$%%%%$&$+%7#7#8$8$+$+$?$8$8$8$8$9$8$+$&#&$&$&#6'+'&$9$7$7$9",
            "post_date": "2013-08-08 02:37:27"
        },
        {
            "playerCommentId": 46,
            "playerId": 14,
            "userName": "unknown",
            "comment": "huan",
            "post_date": "2013-06-08 21:56:34"
        },
        {
            "playerCommentId": 45,
            "playerId": 14,
            "userName": "unknown",
            "comment": "fff",
            "post_date": "2013-06-08 21:55:40"
        },
        {
            "playerCommentId": 43,
            "playerId": 14,
            "userName": "unknown",
            "comment": "rrrrrrrr",
            "post_date": "2013-06-07 01:04:31"
        },
        {
            "playerCommentId": 42,
            "playerId": 14,
            "userName": "unknown",
            "comment": "eeeeeee",
            "post_date": "2013-06-07 01:04:08"
        },
        {
            "playerCommentId": 41,
            "playerId": 14,
            "userName": "unknown",
            "comment": "trst",
            "post_date": "2013-06-07 01:03:59"
        },
        {
            "playerCommentId": 40,
            "playerId": 14,
            "userName": "unknown",
            "comment": "",
            "post_date": "2013-06-06 07:52:35"
        }
    ]
}
```

##13 : Get player statistics  
------------------------
###URL:   
```
/vizoal/services/playerStatistics/{player_id}

Example: /vizoal/services/playerStatistics/1205
```

###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
 
### Response
```

{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ip-172-31-12-36",
            "duration": 18
        }
    },
    "result": {
        "playerId": null,
        "appearance": "32",
        "manOfTheMatch": "12",
        "rating": "8.63",
        "goals": "39",
        "assists": "10",
        "yellowCards": "4",
        "redCards": "1",
        "passSuccessPercentage": "81.7%",
        "goalsPerGame": "1.2",
        "shotsPerGame": "28",
        "shotsOnTargetPerGame": "3.3",
        "dribblePerGame": "2.4",
        "tacklesPerGame": "0.7",
        "interceptionPerGame": "0.1",
        "clearancePerGame": "0.4",
        "arialWonPerGame": "1.8",
        "foulPerGame": "0.8"
    }
}
    
```

##14 : Country logo url  
------------------------
###URL:   /vizoal/image/android/country_logo_profile/{density}/{fm_id}.png

Example: http://api.vizoal.com/vizoal/image/android/country_logo_profile/2.0/796.png


##15 : Top League List

###URL:   
```
/vizoal/services/topleaguelist

```

###Method			
	GET
				
###Header Parameters		
	1) Content-Type = application/json 
 
### Response
```

{
    "status": {
        "code": "200",
        "message": "success",
        "errors": [],
        "debug": {
            "build": "1.0",
            "serverName": "ethan",
            "duration": 478
        }
    },
    "result": [
        {
            "leagueId": 182,
            "name": "World Cup 2014",
            "nationality": 287,
            "nationalityName": "FIFA",
            "fmId": 1301385,
            "sort": 1,
            "currentRound": 0,
            "maxRound": 0,
            "liveMatches": 0,
            "matchdaySettingId": 1,
            "matchdayDisplay": {
                "1": "Group_matchday 1",
                "2": "Group_matchday 2",
                "3": "Group_matchday 3",
                "4": "Group_matchday 4",
                "5": "Group_matchday 5",
                "6": "Group_matchday 6",
                "7": "Round_of_16_first_leg",
                "8": "Round_of_16_Second_leg",
                "9": "Quarter_finals_first_leg",
                "10": "Quarter_finals_second_leg",
                "11": "Final"
            },
            "version": 1
        },
        {
            "leagueId": 181,
            "name": "Champion League",
            "nationality": 286,
            "nationalityName": "UEFA",
            "fmId": 1301394,
            "sort": 0,
            "currentRound": 1,
            "maxRound": 0,
            "liveMatches": 0,
            "matchdaySettingId": 1,
            "matchdayDisplay": {
                "1": "Group_matchday 1",
                "2": "Group_matchday 2",
                "3": "Group_matchday 3",
                "4": "Group_matchday 4",
                "5": "Group_matchday 5",
                "6": "Group_matchday 6",
                "7": "Round_of_16_first_leg",
                "8": "Round_of_16_Second_leg",
                "9": "Quarter_finals_first_leg",
                "10": "Quarter_finals_second_leg",
                "11": "Final"
            },
            "version": 1
        },
        {
            "leagueId": 11,
            "name": "Premier League",
            "nationality": 122,
            "nationalityName": "England",
            "fmId": 11,
            "sort": 1,
            "currentRound": 32,
            "maxRound": 38,
            "liveMatches": 0,
            "matchdaySettingId": 0,
            "matchdayDisplay": null,
            "version": 7
        },
        {
            "leagueId": 17,
            "name": "Bundesliga",
            "nationality": 91,
            "nationalityName": "Germany",
            "fmId": 22,
            "sort": 1,
            "currentRound": 28,
            "maxRound": 34,
            "liveMatches": 0,
            "matchdaySettingId": 0,
            "matchdayDisplay": null,
            "version": 3
        },
        {
            "leagueId": 21,
            "name": "Ligue 1",
            "nationality": 135,
            "nationalityName": "France",
            "fmId": 16,
            "sort": 1,
            "currentRound": 31,
            "maxRound": 38,
            "liveMatches": 0,
            "matchdaySettingId": 0,
            "matchdayDisplay": null,
            "version": 3
        },
        {
            "leagueId": 19,
            "name": "Primera División",
            "nationality": 90,
            "nationalityName": "Spain",
            "fmId": 67,
            "sort": 1,
            "currentRound": 31,
            "maxRound": 32,
            "liveMatches": 0,
            "matchdaySettingId": 0,
            "matchdayDisplay": null,
            "version": 3
        },
        {
            "leagueId": 15,
            "name": "Serie A",
            "nationality": 143,
            "nationalityName": "Italy",
            "fmId": 32,
            "sort": 1,
            "currentRound": 31,
            "maxRound": 31,
            "liveMatches": 0,
            "matchdaySettingId": 0,
            "matchdayDisplay": null,
            "version": 3
        }
    ]
}
    
```
