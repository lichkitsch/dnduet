# _dnduet_ Implementation Plan

```
const user: {
  id: UNIQUE_STRING,
  username: STRING,
  email: STRING,
  password: STRING,
  friends: [user_id],
  gm_status: BOOLEAN,
  admin_status: BOOLEAN,
  characters: [CHARACTER],
  quests: [QUEST]
}
```

```
const character = {
  id: UNIQUE_STRING,
  name: STRING,
  img: STRING,
  level: NUMBER, // 1 to 12
  hp: {
    current: NUMBER,
    max: NUMBER
  },
  stats: {
    str: NUMBER,
    dex: NUMBER,
    con: NUMBER,
    int: NUMBER,
    wis: NUMBER,
    cha: NUMBER,
  },
  inventory: [STRING],
  details: STRING
}
```

```
const quest =  {
  review: STRING,
  npcs: [
    {
      name: STRING,
      level: NUMBER, // 1 to 12
      stats: {
        str: NUMBER,
        dex: NUMBER,
        con: NUMBER,
        int: NUMBER,
        wis: NUMBER,
        cha: NUMBER,
      },
      description: STRING
    }
  ],
  goal: STRING,
  locations: [
    {
      name: STRING,
      imgURL: STRING,
      areas: [
        {
          name: STRING,
          description: STRING,
          obstacles: [STRING]
        }
      ]
    }
  ],
  revelations: [STRING],
  dividends: [STRING]
}
```
