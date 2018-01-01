# FakeBook DB Schema

> Table

* Users
* UsersInfo
* UserImage
* Friends
* FriendsInfo
* TimeLine
* Comments
* Likes



> Users

| NAME         | TYPE      |
| ------------ | --------- |
| id           | INT       |
| useremail    | VARCHAR   |
| username     | VARCHAR   |
| userpassword | VARCHAR   |
| created      | TIMESTAMP |
| updated      | TIMESTAMP |

> UsersInfo

| NAME       | TYPE      |
| ---------- | --------- |
| id         | INT       |
| profile_id | INT       |
| cover_id   | INT       |
| updated    | TIMESTAMP |
| Users_id   | INT       |

> UserImage

| NAME         | TYPE      |
| ------------ | --------- |
| id           | INT       |
| imgPath      | VARCHAR   |
| created      | TIMESTAMP |

> Friends

| NAME       | TYPE      |
| ---------- | --------- |
| Users_id   | INT       |
| Friends_id | INT       |
| created    | TIMESTAMP |

> FriendsInfo

| NAME            | TYPE      |
| --------------- | --------- |
| id              | INT       |
| RequestUser_id  | INT       |
| ResponseUser_id | INT       |
| created         | TIMESTAMP |

> TimeLines

| NAME     | TYPE      |
| -------- | --------- |
| id       | INT       |
| content  | TEXT      |
| created  | TIMESTAMP |
| updated  | TIMESTAMP |
| imgPath  | VARCHAR   |
| Users_id | INT       |

> Comments

| NAME         | TYPE      |
| ------------ | --------- |
| id           | INT       |
| content      | VARCHAR   |
| created      | TIMESTAMP |
| Users_id     | INT       |
| TimeLines_id | INT       |

> Likes

| NAME         | TYPE      |
| ------------ | --------- |
| id           | INT       |
| Users_id     | INT       |
| TimeLines_id | INT       |
| created      | TIMESTAMP |

