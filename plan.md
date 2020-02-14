# _dnduet_ Implementation Plan

```
user: {
  id: UNIQUE_STRING,
  username: STRING,
  email: STRING,
  password: STRING,
  friends: [user_id],
  gm_status: BOOLEAN,
  admin_status: BOOLEAN,
  characters: [
    {
      id: UNIQUE_STRING,
      name: STRING,
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
  ],
  quests: [
    {
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
  ]
}
```
