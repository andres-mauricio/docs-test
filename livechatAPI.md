# REST API

The REST API allows you to control and extend Rocket.Chat with ease.

> **This API is a work in progress, so feel free to test, ask us questions, and submit Pull Requests!**

If you are an end-user and not a dev or a tester, [create a New Feature Request](https://forums.rocket.chat/c/feature-requests) to request new APIs -- and consider [making a donation](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZL94ZE6LGVUSN) to the project.

> All API calls in the documentation are made using `curl`. However, you are free to use Java / Python / PHP / Golang / Ruby / Swift / Objective-C / Rust / Scala / C\# or any other programming languages.

## Production Security Concerns

When calling a production Rocket.Chat server, ensure it is running via HTTPS and has a valid SSL Certificate. The login method requires you to post your username and password in plaintext, which is why we highly suggest only calling the REST login API over HTTPS. Also, few things to note:

* Only call via HTTPS
* Implement a timed authorization token expiration strategy
* Ensure the calling user only has permissions for what they are calling and no more

### Miscellaneous Information (work in progress)

| Url | Short Description | Details Page |
| :--- | :--- | :--- |
| `/api/info` | Information about the Rocket.Chat server. | [Link](methods/miscellaneous/info.md) |
| `/api/v1/directory` | Search by all users and channels available on server. | [Link](methods/miscellaneous/directory.md) |
| `/api/v1/shield.svg` | Gets the shield svg\(badge\) to add in your website. | [Link](methods/miscellaneous/shield-svg.md) |
| `/api/v1/spotlight` | Searches for users or rooms that are visible to the user. | [Link](methods/miscellaneous/spotlight.md) |
| `/api/v1/statistics` | Statistics about the Rocket.Chat server. | [Link](methods/miscellaneous/statistics.md) |
| `/api/v1/statistics.list` | Selectable statistics about the Rocket.Chat server. | [Link](methods/miscellaneous/statistics-list.md) |

### RealTime Monitoring

| Url | Short Description | Details Page |
| :--- | :--- | :--- |
| `/livechat/analytics/dashboard/conversation-totalizers` | conversation totalizer| [Link] (#)|
| `/livechat/analytics/dashboard/agent-productivity-totalizers` | agent productivity totalizers | [Link](#)|
| `/livechat/analytics/dashboard/chats-totalizers` | chats totalizers | [Link](#)|
| `/livechat/analytics/dashboard/charts/chats` | chats chart | [Link](#)|
| `/livechat/analytics/dashboard/charts/chats-per-agent` | chats per agent chart | [Link](#)|
| `/livechat/analytics/dashboard/charts/agents-status | agent status chart | [Link](#)|
| `/livechat/analytics/dashboard/charts/chats-per-department` | chats per department chart | [Link](#)|
| `/livechat/analytics/dashboard/charts/timings` | timings | [Link](#)|


### dashboard

| Url | Short Description | Details Page |
| :--- | :--- | :--- |
| `/livechat/analytics/dashboard/conversation-totalizers` | conversation totalizer| [Link] (#)|
| `/livechat/analytics/dashboard/agent-productivity-totalizers` | agent productivity totalizers | [Link](#)|
| `/livechat/analytics/dashboard/chats-totalizers` | chats totalizers | [Link](#)|
| `/livechat/analytics/dashboard/charts/chats` | chats chart | [Link](#)|
| `/livechat/analytics/dashboard/charts/chats-per-agent` | chats per agent chart | [Link](#)|
| `/livechat/analytics/dashboard/charts/agents-status | agent status chart | [Link](#)|
| `/livechat/analytics/dashboard/charts/chats-per-department` | chats per department chart | [Link](#)|
| `/livechat/analytics/dashboard/charts/timings` | timings | [Link](#)|

### Agents

| Url | Short Description | Details Page |
| :--- | :--- | :--- |
| `/livechat/analytics/agents/average-service-time` | agent average service time| [Link] (#)|
| `/livechat/analytics/agents/total-service-time` | agent total service time | [Link](#)|
| `/livechat/analytics/agents/available-for-service-history` | ## | [Link](#)|

### Departments

| Url | Short Description | Details Page |
| :--- | :--- | :--- |
| `/livechat/analytics/departments/ammount-of-chats` | ammount of chats | [Link] (#)|
| `/livechat/analytics/departments/average-service-time` | average service time | [Link] (#)|
| `/livechat/analytics/departments/average-chat-duration-time` | average chats duration | [Link] (#)|
| `/livechat/analytics/departments/total-service-time` | total service time | [Link] (#)|
| `/livechat/analytics/departments/average-waiting-time` |avg waiting time | [Link] (#)|
| `/livechat/analytics/departments/total-transferred-chats` | total transferred chats| [Link] (#)|
| `/livechat/analytics/departments/total-abandoned-chats` | total abandoned chats | [Link] (#)|
| `/livechat/analytics/departments/percentage-abandoned-chats` | percentage of abandoned chats | [Link] (#)|

### Livechat

| Url | Short Description | Details Page |
| :--- | :--- | :--- |
| `/api/v1/livechat/inquiries.list` | Retrieves a list of open inquiries. | [Link](methods/livechat/inquiries.md#inquiries-list) |
| `/api/v1/livechat/inquiries.take` | Take an open inquiry. | [Link](methods/livechat/inquiries.md#livechat-take-inquiry) |
| `/api/v1/livechat/rooms` | Retrieves a list of livechat rooms. | [Link](methods/livechat/rooms.md) |


* [rocketchat-clojure](https://github.com/MalloZup/missile)
